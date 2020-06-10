// 열거형으로 월~토요일까지를 영어로 화면에 출력하시오.  
   
#include <stdio.h>    
enum days { MON, TUE, WED, THU, FRI, SAT };  // days를 열거형을 선언합니다.  
  
char *days_name[] = {  
	"Monday", "Tuesday", "Wednesday", "Thursday", "Friday",  
	"Saturday"     
};    
  
int main(void)  
{  
	int i;
	for(i=0; i<6; i++){ //  for문을 이용해 열거형으로 선언한 배열을 출력합니다.  
		printf("%s\n",days_name[i]);  
	}  
	  
	return 0;  
}  
