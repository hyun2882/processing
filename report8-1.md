1. 숫자 20,30,40을 파일 data.txt에 저장하시오.
2. 이 값을 읽고 더해서 화면에 출력하시오.


#include<stdio.h>
int main(void){
	int a, b, c; 
	int sum = 0;
	FILE *fp;
	
	fp=fopen("c:\\temp\\dat.txt", "r");
	fscanf(fp, "%d%d%d", &a, &b, &c);
	fclose(fp);
	
	sum = a + b + c;
	printf("%d", sum);
}
