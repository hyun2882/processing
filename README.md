# processing1

void setup() {
  size(500, 500);
}
int h=0;
void draw() {
  background(0); // black 255-white
  fill(0, 0, 255);
  ellipse(h++, 250, 100, 100);
  if (h>500) h=0;
}

첫번째 장에서 선택한 코드는 공이 좌우로 반복하는 코드입니다. 

설명 :  위 코드는 파란색 공이 왼쪽에서 오른쪽으로 이동하다가 끝 지점에 도달하면 다시 처음으로 이동하는 코드입니다.


# processing2


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

제가 두번째 장에서 선택한 소스코드는 한글배너 만들기 입니다.

설명 : 위 코드는 한글 배너가 위에서 아래로 이동하는데 제가 누른 숫자 크기에 따라 속도가 변하는 코드입니다.

# processing3

float x, y;
float angle1 = 0.0;
float angle2 = 0.0;
float segLength = 100;

void setup() {
  size(640, 360);
  strokeWeight(30);
  stroke(255, 160);

  x = width * 0.3;
  y = height * 0.5;
}

void draw() {
  background(0);

  angle1 = (mouseX/float(width)) * -PI;
  angle2 = (mouseY/float(height)) * PI;

  pushMatrix();
  segment(x, y, angle2); 
  segment(segLength, 0, angle1);.
  popMatrix();
}

void segment(float x, float y, float a) {
  translate(x, y);
  rotate(a);
  line(0, 0, segLength, 0);
}

세번째 장에서는 움직이는 팔에서 제가 수정한 코드입니다.

설명 : 위 코드는 두가지의 각도를 설정해주고 마우스의 움직임에 따라 팔 모양처럼 생긴 도형이 움직이는 코드입니다.

# processing 4

void setup() {
  size(500, 500);
  rectMode(CENTER);
  ellipseMode(CENTER);
}
void draw() {
  rect(250, 250, 300, 100);
  ellipse(150,300,40,40);
  ellipse(150,300,20,20);
  ellipse(350,300,40,40);
  ellipse(350,300,20,20);
  rect(130,240,50,60);
  rect(275,230,210,40);
  line(170,220,380,220);
  line(275,210,275,250);
  line(222.5,210,222.5,250);
  line(327.5,210,327.5,250);
}

네번째 장에서는 제가 직접 만든 도형입니다.

설명 : 사각형과 원을 이용해 버스의 옆면을 표현한 코드입니다.

# processing 5

PGraphics pg;
PImage bg;

void setup() {
  size(640, 360);
  pg = createGraphics(400, 200);
  bg = loadImage("moonwalk.jpg"); // 배경에 달을 걷는 사진을 삽입해주었습니다.
}

void draw() {
  background(bg); // 배경에 달을 걷는 사진을 삽입해주었습니다.
  fill(0, 12);
  rect(0, 0, width, height);
  fill(255);
  noStroke();
  ellipse(mouseX, mouseY, 80, 80); // 원의 크기를 동일하게 키워주었습니다.

  pg.beginDraw();
  pg.background(127);  //색을 회색으로 변경하였습니다.
  pg.fill(255); //구의 색깔을 바깥과 동일하게 흰색으로 채워주었습니다.
  pg.stroke(255);
  pg.ellipse(mouseX-120, mouseY-60, 80, 80);  // 원의 크기를 동일하게 키워주었습니다.
  pg.endDraw();

  image(pg, 120, 60);
}

설명 : PGraphics의 예제에서 달 사진을 삽입하고 구의 크기와 색깔을 바꿔준 코드입니다.




