# Sprint-1 
#include <stdio.h>

int main(void) {
    int num1, num2;
    char opcao;

    printf("Introduza dois numeros inteiros separados por espaco: ");
    scanf("%d %d", &num1, &num2);

    // Calculo do valor medio
    // BUG: A divisao abaixo nao devolve o valor decimal correto
    double media = (num1 + num2) / 2.00;
    printf("A media dos numeros e: %.2f\n", media);

    printf("Deseja continuar? (S/N): ");
    // BUG: O scanf abaixo vai ler o '\n' que ficou no buffer de entrada!
    scanf(" %c", &opcao);

    printf("Opcao selecionada: '%c'\n", opcao);

    return 0;
}
