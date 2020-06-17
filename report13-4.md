// 주사위를 6000번 던질때 각 숫자들이 나오는 횟수 계산.   

#include<stdio.h>  
#include<time.h>  
  
int main(void){  
	int i, r;  
	int h[6];  
	srand(time(NULL)); // 매 순간 숫자들을 달라지게 하기 위해 time()함수를 사용함.  
	for(i = 0; i< 6000; i++){
		r = rand(); // 변수 r에 난수를 넣음.  
		r = r % 6; // 난수 r을 6으로 나누었을때 나머지를 계산함.  
		h[r] = h[r] + 1;   
	}  
	for(i = 0; i < 6; i++){  
		printf("[%d] = %d\n", i+1, h[i]);  // 각 숫자들이 나오는 횟수 출력.  
	}  
}   
