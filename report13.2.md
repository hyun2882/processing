// 스택 자료구조 구현  
#include<stdio.h>  
int s[1000];  // 정수 1000개를 넣을 수 있는 배열 선언.  
int sp = 0;  
void push(int a){ // 배열에 수를 넣는 push 함수 구현.  
	s[sp] = a; // s[0]부터 순서대로 숫자들을 push함.  
	sp++;  
}  
  
int pop(){  // pop함수 구현.  
	sp--;   
	return (s[sp]); // 이 코드에서 s[2]부터 차례대로 숫자들을 빼낸다.  
}  
void main(){    
	push(2);   
	push(7);      
	push(1);    
	printf("%d\n", pop());  
	printf("%d\n", pop());   
	printf("%d\n", pop());   
}   
