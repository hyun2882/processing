//정수 5개 작은 수 부터 정렬.

#include<stdio.h> 
void swap(int *a, int *b){ //두 수의 위치를 바꾸는 swap함수 구현.  
	int temp;  
	temp = *a;    
	*a = *b;   
	*b = temp;  
}   
   
int main(void){  
	int i, j;  
	int a[6] = {5, 2, 4, 6, 1, 3}; // 순서를 정렬할 배열 선언  
	
	for(i = 0; i < 6; i++){  
		for(j = 0; j < 5 - i; j++){  
			if(a[j] > a[j+1])  // 큰수부터 정렬하려면 부호를 반대로 바꾸면 됨.  
				swap(&a[j], &a[j+1]);  // 위치를 바꾸는 swap함수로 숫자들을 보냄.  
		}  
	}  
	  
	for(i = 0; i < 6; i++)  
		printf("%d ", a[i]);  // 정리된 배열 출력.  
}  
