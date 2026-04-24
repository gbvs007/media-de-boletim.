#include <stdio.h>

int main() {
    char nome[100];
    double nota1, nota2, resultado;

    printf("Qual seu nome completo: ");
    fgets(nome, 100, stdin); 
    
    printf("Digite a primeira nota: ");
    scanf("%lf", &nota1);

    printf("Digite a segunda nota: ");
    scanf("%lf", &nota2);

    resultado = (nota1 + nota2) / 2;

    printf("\nAluno: %s", nome);
    printf("Média: %.2lf\n", resultado);

    if (resultado >= 7) {
        printf("Situação: Aprovado\n");
    } else if (resultado >= 5) {
        printf("Situação: Recuperação\n");
    } else {
        printf("Situação: Reprovado\n");
    }

    return 0;
}# media-de-boletim.
