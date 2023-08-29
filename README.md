#include <stdio.h>
#include <stdlib.h>
#include <locale.h>

/* run this program using the console pauser or add your own getch, system("pause") or input loop */

int main(int argc, char *argv[]) {
	// Aplicando localidade
	setlocale(LC_ALL, "portuguese");
	
	// Aplicação de variaveis
	int OP;
	float soma1, soma2, resultsoma, mult1, mult2, resultmult, div1, div2, resultdiv, sub1, sub2, resultsub;
	
	//Codigo Menu
	puts ("\t\t\t============Bem-Vindo==========\n");
	puts ("\t\t\t|\t                      |\n");
	puts ("\t\t\t|\t 1 - Soma             |\n");  
	puts ("\t\t\t|\t 2 - Multiplicação    |\n");
	puts ("\t\t\t|\t 3 - Divisão          |\n");
	puts ("\t\t\t|\t 4 - Subtração        |\n");
	puts ("\t\t\t|\t                      |\n");
	puts ("\t\t\t===============================\n");
	puts ("\n\n");
	puts ("\t\t\tSelecione uma das opções acima: ");
	scanf("\t\t\t%d", &OP);
	//Opções do Menu
	switch(OP){
		case 1:
			puts("\t\t\tVoce selecionou a opção 1 - Soma.\n");
			puts("\t\t\tInsira o PRIMEIRO numero que deseja somar:\n");
			scanf("%f", &soma1);
			puts("\t\t\tInsita o SEGUNDO numero que deseja somar:\n");
			scanf("%f", &soma2);
			
			//Calculo dos valores
			
			resultsoma = soma1 + soma2;
			
			//Passando o resultado
			
			printf("\t\t\tO resultado da sua soma é:%f", resultsoma);
			
			break;
			case 2:
				puts("\t\t\tVoce selecionou a opção 2 - Multiplicação.\n");
				puts("\t\t\tInsira o PRIMEIRO numero que deseja multiplicar:\n");
				scanf("\t\t\t%f", &mult1);
				puts("\t\t\tInsira o SEGUNDO numero que deseja multiplicar:\n");
				scanf("\t\t\t%f", &mult2);
				
				//Calculo dos Valores
				
				resultmult = mult1 * mult2;
				
				//Passando o resultado
				
				printf("\t\t\tO resultado da sua Multiplicação é:%f", resultmult);
				
				break;
				case 3:
					puts("\t\t\tVoce selecionou a opção 3 - Divisão.\n");
					puts("\t\t\tInsira o PRIMEIRO numero que deseja dividir:\n");
					scanf("\t\t\t%f", &div1);
					puts("\t\t\tInsira o SEGUNDO numero que deseja dividir:\n");
					scanf("\t\t\t%f", &div2);
					
					//Calculo dos Valores
					
					resultdiv = div1 / div2;
					
					//Passando o resultado
					
					printf("\t\t\tO resultado da sua Divisão é:%f", resultdiv);
					
					break;
					case 4:
						puts("\t\t\tVoce selecionou a opção 4 - Subtração.\n");
						puts("\t\t\tInsira o PRIMEIRO numero que deseja Subitrair:\n");
						scanf("\t\t\t%f", &sub1);
						puts("\t\t\tInsira o SEGUNDO numero que deseja Subtrair:\n");
						scanf("\t\t\t%f", &sub2);
						
						//Calculo de Valores
						
						resultsub = sub1 - sub2;
						
						//Passando o resultado
						
						printf("\t\t\tO resultado da sua Subtração é:%f", resultsub);
						break;
						
						//Caso digite numero invalido
						default:
							puts("\t\t\tOpção inserida invalida, tente novamente.");
							break;
	}
	
	return 0;
}
