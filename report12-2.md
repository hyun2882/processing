// 함수로 3명의 구조체 배열을 전달하고 화면에 출력하시오. 
#include <stdio.h>  
typedef struct _user{  // 정보를 저장할 구조체를 만듭니다.  
	char name[20];  
	int age;  
	char number[20];  
	char e_mail[30];  
} user;  
    
void printUser(user a){  // 구조체를 출력해주는 함수를 만듭니다.  
	printf("이름 : %s \n", a.name);  
	printf("나이 : %d \n", a.age);  
	printf("번호 : %s \n", a.number);  
	printf("e-mail : %s \n\n", a.e_mail);  
}  
int main(void){  
	user a[3] = {  //구조체에 정보를 저장합니다.  
		{"SangHyun", 24, "010-7659-9427", "sosemfdkshk1@naver.com"},  
		{"DoHyun", 25, "010-8945-5125", "dohyun23@naver.com"},  
		{"MinJi", 21, "010-4575-5586", "min23@naver.com"}  
	};  
	int i;  
	for(i=0; i<3; i++){  //for문을 이용하여 함수를 통해 구조체를 출력합니다.  
		printUser(a[i]);  
	}  
  
	return 0;  
}  
