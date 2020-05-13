//매크로 함수로 실수로 된 반지름을 입력하면 면적을 계산하는 프로그램을 작성하시오.

#include<stdio.h>
#define PI 3.14
#define AREA(r) PI*r*r

int main(void){
	int r;
	printf("반지름을 입력하시오: ");
	scanf("%d", &r);
	printf("원의 면적 : %lf", AREA(r));
	
	return 0;
}
