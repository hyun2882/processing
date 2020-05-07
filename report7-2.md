정수 2x2 매트릭스 3개를 선언하고, 이 값을 더해서 화면에 출력하시오.
#include<stdio.h>
int main(void){
	int i, j;
	int mat1[2][2] = {{1,2}, {3,4}};
	int mat2[2][2] = {{2,3}, {4,5}};
	int mat3[2][2];
	
	for(i = 0; i <= 1; i++){
		for(j = 0; j <= 1; j++){
			mat3[i][j] = mat1[i][j] + mat2[i][j];
			printf("%d ", mat3[i][j]);
		}
		printf("\n");
	}
}
