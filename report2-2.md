PFont f;
void setup() {
  size(800, 300);
  f = createFont("굴림", 64);
  textFont(f);
}
int h, sp=1;
void draw() {
  fill(0);
  background(128);
  text("안동대 컴공 사랑합니다", 50, h);
  if (h>300) h=0;
  h = h+1*sp;
}
void keyPressed() {
  sp = key - '0';
}

