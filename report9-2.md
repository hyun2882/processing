/* 주사위를 6,000회 던질 때 1부터 6이 나올 확률 */

#include<stdio.h>  
#include<time.h> //time 함수를 사용하기 위해 선언해줍니다.  
int main(void){  
	int i, n;  
	float h[6]={}; //확률을 계산하기 위해 실수로 선언합니다.  
	srand(time(NULL)); //실행할 때마다 다른 숫자가 나오게 하기 위하여 time()함수를 사용합니다.  
	for(i = 0; i < 6000; i++){  
		h[rand() % 6] += 1; // 6000천번 실행하면서 나머지를 계산해줍니다.  
	}  
	for(i = 0; i < 6; i++){  
		printf("%d : %lf \n", i+1, h[i]/6000*100); // 1부터 6까지 나온 횟수의 확률을 계산합니다.  
	}   
	   
	return 0;  
}
