//명령행 매개변수로 +,-,*,/ 를 할 수 있는 계산기를 프로그래밍하시오.   
  
#include<stdio.h>    
int main(int n, char *v[]){    
	// 11-1     10     +      20  
	// v[0]    v[1]   v[2]   v[3]    
	switch(v[2][0]){  
		case '+' : printf("%d\n", atoi(v[1]) + atoi(v[3]));  
		break;  
		case '-' : printf("%d\n", atoi(v[1]) - atoi(v[3]));  
		break;  
		case '*' : printf("%d\n", atoi(v[1]) * atoi(v[3]));  
		break;  
		case '/' : printf("%d\n", atoi(v[1]) / atoi(v[3]));  
		break;  
	}  
  
}  
