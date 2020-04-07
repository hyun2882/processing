#include<stdio.h>

void main(){
	int r;
	double a;
	double pi = 3.14;
	
	printf("반지름을 입력하시오 : ");
	scanf("%d", &r);
	a = pi*r*r;
	printf("원의 면적은 %.2f 입니다.", a);
	
}
