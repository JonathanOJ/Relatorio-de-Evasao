#include <stdio.h>
int main(void){
	
	float alunos18, evasao18;
	float alunos19, evasao19;
	float alunos20, evasao20;
	float alunos21, evasao21;
	int totAlunos=0, totEvadi=0, ano;
	int menorEva=1000, maiorEva=0;
	int anoMenorEva=0, anoMaiorEva=0;
	
	while(ano != -1){
		printf("Confirme o ano: ");
		scanf("%d", &ano);
		
		if(ano == 2018){
			printf("Quantos alunos entraram no ano: ");
				scanf("%f", &alunos18);
				totAlunos = totAlunos + alunos18;
			printf("Quantos alunos evadiram no ano: ");
				scanf("%f", &evasao18);
				totEvadi = totEvadi + evasao18;
						
			if(menorEva >= evasao18){
				menorEva = evasao18;
				anoMenorEva = ano;
			}
			if(maiorEva <= evasao18){
				maiorEva = evasao18;
				anoMaiorEva = ano;
			}
				
			while(ano != -1){
				printf("Confirme o ano: ");
				scanf("%d", &ano);
				
				if(ano == 2019){
					printf("Quantos alunos entraram no ano: ");
						scanf("%f", &alunos19);
						totAlunos = totAlunos + alunos19;
					printf("Quantos alunos evadiram no ano: ");
						scanf("%f", &evasao19);
						totEvadi = totEvadi + evasao19;
						
					if(menorEva >= evasao19){
						menorEva = evasao19;
						anoMenorEva = ano;
					}
					if(maiorEva <= evasao19){
						maiorEva = evasao19;
						anoMaiorEva = ano;
					}
					
					while(ano != -1){
						printf("Confirme o ano: ");
						scanf("%d", &ano);
				
						if(ano == 2020){
							printf("Quantos alunos entraram no ano: ");
								scanf("%f", &alunos20);
								totAlunos = totAlunos + alunos20;
							printf("Quantos alunos evadiram no ano: ");
								scanf("%f", &evasao20);
								totEvadi = totEvadi + evasao20;
								
							if(menorEva >= evasao20){
								menorEva = evasao20;
								anoMenorEva = ano;
							}
							if(maiorEva <= evasao20){
								maiorEva = evasao20;
								anoMaiorEva = ano;
							}
									
							while(ano != -1){
								printf("Confirme o ano: ");					
								scanf("%d", &ano);
							
								if(ano == 2021){
									printf("Quantos alunos entraram no ano: ");
										scanf("%f", &alunos21);
										totAlunos = totAlunos + alunos21;
									printf("Quantos alunos evadiram no ano: ");
										scanf("%f", &evasao21);
										totEvadi = totEvadi + evasao21;
										
								if(menorEva >= evasao21){
									menorEva = evasao21;
									anoMenorEva = ano;
								}
								if(maiorEva <= evasao18){
									maiorEva = evasao18;
									anoMaiorEva = ano;
								}
		
					}else{
						printf("O ano informado esta invalido. Confirme novamente.\n");
						}			
				}
				}else{
					printf("O ano informado esta invalido. Confirme novamente.\n");
					}			
			}			
			}else{
				printf("O ano informado esta invalido. Confirme novamente.\n");
				}			
		}
		}else{
			printf("O ano informado esta invalido. Confirme novamente.\n");
			}		
	}
	float media_Eva, porcent_ent, porcent_eva;
	
	media_Eva = (evasao18 + evasao19 + evasao20 + evasao21)/4;
	
	printf("Periodo .....................................: 2018 - 2021\n\n");
	porcent_ent = alunos18 * 100/totAlunos; 
	printf("Quantidade de alunos que entraram em 2018....: %.f (%.2f%%)\n", alunos18, porcent_ent);
	porcent_ent = alunos19 * 100/totAlunos; 
	printf("Quantidade de alunos que entraram em 2019....: %.f (%.2f%%)\n", alunos19, porcent_ent);
	porcent_ent = alunos20 * 100/totAlunos; 
	printf("Quantidade de alunos que entraram em 2020....: %.f (%.2f%%)\n", alunos20, porcent_ent);
	porcent_ent = alunos21 * 100/totAlunos; 
	printf("Quantidade de alunos que entraram em 2021....: %.f (%.2f%%)\n\n", alunos21, porcent_ent);
	
	porcent_eva = evasao18 * 100/totEvadi;
	printf("Quantidade de alunos que evadiram em 2018....: %.f (%.2f%%)\n", evasao18, porcent_eva);
	porcent_eva = evasao19 * 100/totEvadi;
	printf("Quantidade de alunos que evadiram em 2019....: %.f (%.2f%%)\n", evasao19, porcent_eva);
	porcent_eva = evasao20 * 100/totEvadi;
	printf("Quantidade de alunos que evadiram em 2020....: %.f (%.2f%%)\n", evasao20, porcent_eva);
	porcent_eva = evasao21 * 100/totEvadi;	
	printf("Quantidade de alunos que evadiram em 2021....: %.f (%.2f%%)\n\n", evasao21, porcent_eva);	
	
	printf("Ano que houve menor evasao...................: %d\n", anoMenorEva);
	printf("Ano que houve maior evasao...................: %d\n", anoMaiorEva);
	printf("Media de evasao do periodo...................: %.2f\n", media_Eva);	
}