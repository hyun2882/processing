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

설명
1. 배경을 500,500으로 설정해줍니다.
2. 잔상을 없애기 위해 배경을 검정색으로 해줍니다.
3. 공의 색깔을 파란색으로 채워줍니다.
4. 공을 만들어주는 ellipse에 세로위치는 250으로 고정해주고 가로위치를 h++로 이동시켜줍니다.
5. 공의 크기는 100,100으로 설정합니다.
6. 공의 위치가 오른쪽에 다달했을시에는 공의 위치를 다시 처음으로 이동시켜줍니다.
