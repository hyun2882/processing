// 두 수를 교환하는 swap 프로그램 작성  

#include 
void swap(int *a, int *b){  //swap 함수 구현 포인터로 받음  
	int temp;  //a를 저장할 공간인 temp변수 선언  
	temp = *a;   
	*a = *b;  
	*b = temp;   
}  
int main(void){   
	int a=2, b=5;   
	swap(&a, &b); // 보낼때는 주소를 보내야함.  
	printf("%d %d\n", a, b);   
	   
	return 0;   
}    
