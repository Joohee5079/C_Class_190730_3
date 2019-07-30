# C_Class_190730_3
숫자열 입력?


#include <stdio.h>
void main()
{
	char a[10] = {'0', '一', '二', '三', '四', '五', '六', '七', '八', '九'};
	//한자 코드 인식을 못 함.
	//유니코드를 사용해야 함.
	int num, m, n, x = 100;
	printf("숫자열을 입력하세요. : ");
	scanf_s("%d", &num);
	while (x >= 1)
	{
		m = num / x; //입력값 num에 x값 100을 나눈 몫과 나머지
		n = num % x;
		printf("%c", a[m]); //m(몫)의 값 숫자인 인덱스 출력
		x /= 10;
	}
	printf("\n");
}
