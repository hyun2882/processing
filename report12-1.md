// 구조체로 이름/ 나이/ 폰번호/ 이메일을 정의하고 3명의  
// 데이터를 구조체 배열에 초기화하고 화면에 출력하시오.   
  
#include <stdio.h>  
typedef struct _user{  // 정보를 저장하는 구조체를 만듭니다.  
	char name[20];  
	int age;  
	char number[20];  
	char e_mail[30];  
} user;  //typedef를 이용하여 구조체의 이름을 user로 정의합니다.  

int main(void){  
	user a[3] = {  // 구조체에 정보를 입력합니다.  
		{"SangHyun", 24, "010-7659-9427", "sosemfdkshk1@naver.com"},  
		{"DoHyun", 25, "010-8945-5125", "dohyun23@naver.com"},  
		{"MinJi", 21, "010-4575-5586", "min23@naver.com"}  
	};  
	 
	int i;
	for(i = 0; i < 3; i++){ // for문을 이용하여 구조체를 출력합니다.  
		printf("이름 : %s \n", a[i].name);
		printf("나이 : %d \n", a[i].age);
		printf("번호 : %s \n", a[i].number);
		printf("e-mail : %s \n\n", a[i].e_mail);
	}
	
	
	return 0;
}
