// for문을 활용해 100이하의 자연수 중 3의 배수를 출력하기.
#include<stdio.h>
void main()
{
	printf("100이하의 수 중에 3의 배수를 출력하시오 \n\n"); 
	int i = 1; 
	
	for(i = 1; i <= 100; i++)
	{
		if(i % 3 == 0)
		{
			printf("%d ", i);
		}
		
	}
}
