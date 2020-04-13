#include <stdio.h>
int main(void)
{
	int score;
	
	printf("점수를 입력하세요 : ");
	scanf("%d", &score);
	    
	switch (score/10)
	{
  case 10 :
	case 9 :
		printf("A학점 입니다. ");
		break;
	case 8 :
		printf("B학점 입니다. ");
		break;
	case 7 :
		printf("C학점 입니다. ");
		break;
	case 6 :
		printf("D학점 입니다. ");
		break;
	default :
		printf("F학점 입니다. ");
		break;
	}
}
