#include<stdio.h>
void main(){
	int grade;
	printf("성적을 입력하시오 : ");
	scanf("%d", &grade);
	
	if(grade>=90)
		printf("A 학점 \n");
	else if(grade>=80)
		printf("B 학점 \n");
	else if(grade>=70)
		printf("C 학점 \n");
	else if(grade>=60)
		printf("D 학점 \n");
	else
		printf("F 학점 \n");
		
}
