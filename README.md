#define _CRT_SECURE_NO_WARNINGS
//Перевод числа в 3 систему счисления

#include<stdio.h>

int main() {
	int x = 0, y = 0, z = 1;
	printf("Input number ");
	scanf("%d", &y);


	if (y < 0) {
		printf("No solutions");
	}
	else {
		while (y) {
			x = x + (y % 3) * z;
			z = z * 10;
			y = y / 3;
		}
		printf("%d", x);
	}
	return 0;
}
