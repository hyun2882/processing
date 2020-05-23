// 메모리에 두 수를 저장하고 사칙연산을 하는 함수기반 프로그램. 
#include <stdio.h>
float add(float i, float j){
	return i + j;
}
float minus(float i, float j){
	return i - j;
}
float multifly(float i, float j){
	return i * j;
}
float division(float i, float j){
	return i / j;
}
int main(void){
	float a, b;
	printf("두 수를 입력하세요: ");
	scanf("%f%f", &a, &b); 
	printf("덧셈 결과 : %.3lf\n", add(a, b));
	printf("뺄셈 결과 : %.3lf\n", minus(a, b));
	printf("곱셈 결과 : %.3lf\n", multifly(a, b));
	printf("나눗셈 결과 : %.3lf\n", division(a, b));
	return 0;
}
