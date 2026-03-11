```C
#include <stdio.h>
#include <stdlib.h>

void soma(float a, float b) {
    printf("Resultado: %.2f\n", a + b);
}
void subtracao(float a, float b) {
    printf("Resultado: %.2f\n", a - b);
}
void multi(float a, float b) {
    printf("Resultado: %.2f\n", a * b);
}
void divisao(float a, float b) {
    if(b != 0) {
        printf("Resultado: %.2f\n", a / b);
    } else {
        printf("Nao e possivel dividir por zero!");
    }
}
int main() {
    float num1; 
	float num2;
    int opcao = -1;

    while (opcao != 0) {
        printf("\nCALCULADORA\n");
        printf("1 - Soma\n");
        printf("2 - Subtracao\n");
        printf("3 - Multiplicacao\n");
        printf("4 - Divisao\n");
        printf("0 - Sair\n");
        printf("\nQual operacao deseja realizar?\n");
        scanf("%d", &opcao);
        
        if(opcao == 1) {
        	printf("\nEscolheu Adicao: \n");
        	printf("\nPrimeiro operador da soma: ");
            scanf("%f", &num1);

            printf("\nSegundo operador da soma: ");
            scanf("%f", &num2);
		}
		if(opcao == 2) {
        	printf("\nEscolheu Subtracao: \n");
        	printf("\nPrimeiro operador da subtracao: ");
            scanf("%f", &num1);

            printf("\nSegundo operador da subtracao: ");
            scanf("%f", &num2);
		}
		if(opcao == 3) {
        	printf("\nEscolheu Multiplicacao: \n");
        	printf("\nPrimeiro operador da multiplicacao: ");
            scanf("%f", &num1);

            printf("\nSegundo operador da multiplicacao: ");
            scanf("%f", &num2);
		}
		if(opcao == 4) {
        	printf("\nEscolheu Divisao: \n");
        	printf("\nPrimeiro operador da divisao: ");
            scanf("%f", &num1);

            printf("\nSegundo operador da divisao: ");
            scanf("%f", &num2);
		}    		   
        switch(opcao) {
            case 1:
            soma(num1, num2);
            break;

            case 2:
            subtracao(num1, num2);
            break;

            case 3: 
            multi(num1, num2);
            break;

            case 4:
            divisao(num1, num2);
            break;

            case 0:
            printf("Saindo...");
            break;
            
            default:
            printf("Operacao Invalida!!");

        }
    }
    return 0;
}
```C
