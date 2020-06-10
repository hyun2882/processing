// 함수로 3명의 구조체 배열을 포인터로 전달하고 화면에 출력하시오.  
   
#include <stdio.h>  
typedef struct _user{ // 정보를 저장할 구조체를 정의합니다.  
	char name[20];  
	int age;  
	char number[20];  
	char e_mail[30];  
} user;  
  
void printUser(user *p){  // 포인터를 이용해 매개변수를 받아 출력하는 함수를 정의합니다.  
	printf("이름 : %s \n", p->name);  
	printf("나이 : %d \n", p->age);  
	printf("번호 : %s \n", p->number);  
	printf("e-mail : %s \n\n", p->e_mail);  
  
}   
int main(void){  
	user a[3] = {  // 구조체에 저장할 값을 입력합니다.  
		{"SangHyun", 24, "010-7659-9427", "sosemfdkshk1@naver.com"},  
		{"DoHyun", 25, "010-8945-5125", "dohyun23@naver.com"},  
		{"MinJi", 21, "010-4575-5586", "min23@naver.com"}  
	};  
	user *p;  // 구조체 포인터 변수를 정의합니다.  
	
	int i;  
	for(i=0; i<3; i++){  // for문을 이용해 p가 구조체를 가르키도록 하고 그것을 출력하는 함수에 보내 출력합니다.  
		p = &a[i];  
		printUser(p);  
	}  
  
	return 0;  
}  
