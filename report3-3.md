#include<stdio.h>
void main()
{
	char name[20];
	int age;
	float height;
	
	printf("이름을 입력하세요 : ");
	scanf("%s", name);
	printf("나이를 입력하세요 : ");
	scanf("%d", &age);
	printf("키를 입력하세요 : ");
	scanf("%f", &height);
	
	printf("이름 : %s \n", name);
	printf("나이 : %d \n", age);
	printf("키 : %.1f \n", height);
} 
