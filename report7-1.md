실수 { 1.1, 2.2, 3.3, 4.4, 5.5}를 배열에 초기화 하고, 더한 값을 화면에 출력하시오.
#include<stdio.h>
int main(void){
	int i; 
	double dat[5] = {1.1, 2.2, 3.3, 4.4, 5.5};
	double sum = 0;
	for(i = 0; i <= 4; i++){
		sum += dat[i];
	}
	printf("%.1f", sum);
}
