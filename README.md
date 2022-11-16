#include <stdio.h>
#include <stdlib.h>

/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char *argv[]) {
	float vizeNot, finalNot, devamNot;
	float ortalama=0;
	printf("vize notu: ");
	scanf("%f.2", &vizeNot);
	printf("final not: ");
	scanf("%f.2", &finalNot);
	printf("devam not: ");
	scanf("%f.2", &devamNot);
	
	ortalama=((vizeNot/100)*4)+((finalNot/100)*50)+((devamNot/100)*10);
	
	if(ortalama>=50)
	{
		printf("Gectiniz\n");
	}else if(ortalama>=35 && ortalama<50){
		printf("Kosullu gectiniz\n");
	}else{
		printf("Kaldiniz\n");
	}
	printf("Ortalama %.2f", ortalama);
	return 0;
}
