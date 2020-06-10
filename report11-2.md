/* 키보드에서 입력되는 값이 "love"이면 OK를 출력하고 그 외에것은 Try again을 출력하여 다시 입력할 수 있게 하시오 */
#include<stdio.h>  
  
int main(void){  
	int a;  
	char key[80] = "love";  // key라는 변수에 "love"를 넣어줍니다.  
	char str[80];  // 입력받는 문장을 저장할 str을 선언합니다.  
	  
	for(;;){	  // love외에 다른 문장이 들어오면 다시 실행되도록 무한반복을 걸어줍니다.  
	  
	printf("문장를 입력하시오 : ");  
	gets(str);  // 문장을 입력 받습니다.  
	a = strcmp(key, str);  key("love")와 입력받은 문장(str)이 같은지 확인합니다. 같다면 a에는 0이 들어갑니다.  
	   
	if (a == 0){  // 같을시에는 반복문을 탈출합니다.  
		printf("OK");  
		break;  
	}  
	else{  // 그 외의 경우엔 다시 돌아가서 문장을 받습니다.  
		printf("Try again \n\n");  
	}  
}  
	return 0;  
}  
