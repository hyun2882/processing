#include <stdio.h>
int main(void)
{
	int num;
	int sum = 0;
	
	for(num = 1; num <= 1000; num++)
	{
		if ( num % 3 == 0)
		   sum = sum + num;
	}
	printf("1부터 1000까지 3의 배수들의 합은 : %d", sum);
}
