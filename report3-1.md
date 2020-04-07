#include<stdio.h>
void main(){
	char name[];
	int age;
	double height;
	
	printf("이름을 입력하세요 : ");
	scanf("%s", name);
	printf("나이를 입력하세요 : ");
	scnaf("%d", &age);
	printf("키를 입력하세요 : ");
	scnaf("%f", &height);
	
	printf("이름 : %s \n", name);
	printf("나이 : %d \n", age);
	printf("키 : %.2f \n", double);
} 
