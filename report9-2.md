// 주사위를 6,000회 던질 때 1부터 6이 나올 확률
#include<stdio.h>
#include<time.h>
int main(void){
	int i, n;
	int h[6]={};
	srand(time(NULL));
	for(i = 0; i < 6000; i++){
		h[rand() % 6] += 1;
	}
	for(i = 0; i < 6; i++){
		printf("%d : %d\n", i+1, h[i]);
	}
	
	return 0;
}
