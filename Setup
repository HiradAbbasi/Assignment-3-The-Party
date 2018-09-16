int a = 0;
int fade = -10;

Drop[] drops = new Drop[100];

void setup() {
  size(600,600);
  for (int i = 0; i < drops.length; i++) {
    drops[i] = new Drop();
  }
}

void draw() {
  background(255, 255, 0);
  fill(255,51,221);
  textSize(50);
  text("Lets Have a Party!",90,300);
  for (int i = 0; i < drops.length; i++) {
    drops[i].fall();
    drops[i].show();
  }
  fill(255,51,221);
  textSize(25);
  text("Click screen to give presents",120,350);
  textSize(25);
  text("and to show a secret message!",110,375);
  fill(255,0,0,fade);
  textSize(50);
  text("This Party is the best!!",35,200);
  fill(255,51,221);
  textSize(25);
  text("Number of presents:"+ a ,165,400);
}

void mousePressed() {
  fade = fade + 10;
  a += 1;
}
