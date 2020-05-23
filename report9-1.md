/* 메모리에 두 수를 저장하고 사칙연산을 하는 함수기반 프로그램 */

#include <stdio.h>
float add(float i, float j){ // 덧셈 함수
	return i + j;
}
float minus(float i, float j){ // 뺄셈 함수
	return i - j;
}
float multifly(float i, float j){ //곱셈 함수
	return i * j;
}
float division(float i, float j){ //나눗셈 함수
	return i / j;
}

int main(void){
	float a, b; /* 실수를 처리하기 위한 실수 변수를 선언합니다. */
	printf("두 수를 입력하세요: ");
	scanf("%f%f", &a, &b); /*두 수를 입력받아서 메모리에 저장합니다.*/
	printf("덧셈 결과 : %.3lf\n", add(a, b)); /* 각각의 값들을 함수를 이용하여 출력합니다. 시인성을 위해 소수점 3자리까지만 출력합니다.*/
	printf("뺄셈 결과 : %.3lf\n", minus(a, b));
	printf("곱셈 결과 : %.3lf\n", multifly(a, b));
	printf("나눗셈 결과 : %.3lf\n", division(a, b));
	
	return 0;
}
