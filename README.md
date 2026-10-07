# Sprint-1 
#include <stdio.h>
int main (void)
    {   
        int valor;
        float temp;
        printf("Digite um valor inteiro entre 0 e 1023 para ser lido pelo sensor:\n");
        scanf("%d", &valor);

        temp = (260.00*valor)/1023-20;

        printf("a temperatura lida pelo sensor é: %.2lf\n", temp);
    }
