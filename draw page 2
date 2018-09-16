// Daniel Shiffman


class Drop {
  float x;
  float y;
  float z;
  float w;
  float h;
  float i;
  float l;
  float len;
  float yspeed;

  Drop() {
    x  = random(width);
    y  = random(-500, -50);
    w  = random(width);
    h  = random(-500, -50);
    i = random(width);
    l  = random(-500, -50);
    z  = random(0, 20);
    len = map(z, 0, 20, 10, 20);
    yspeed  = map(z, 0, 20, 1, 20);
  }

  void fall() {
    y = y + yspeed;
    h = h + yspeed;
    l = h + yspeed;
  float grav = map(z, 0, 20, 0, 0.2);
    yspeed = yspeed + grav;

    if (y > height) {
      y = random(-200, -100);
      h = random(-200, -100);
      l = random(-200, -100);
      yspeed = map(z, 0, 20, 4, 10);
    }
  }

  void show() {
    float thick = map(z, 0, 20, 1, 3);
    strokeWeight(1.5);
    stroke(0,0,0);
    
    fill(0,255,0);
    ellipse(x, y, 20, 20);
    fill(0,0,255);
    rect(w, h, 20, 20);
    strokeWeight(5);
    stroke(255,0,0);
    line(x,l,x,l+len);
  }
}
