### CALCULADORA COM MENU



#include<stdio.h>
#include<stdlib.h>
#include<locale.h>

void main (){

//PARA USAR ACENTOS

setlocale(LC_ALL, "");

//ALGORITMO - CALCULADORA COM MENU

float valor1, valor2;
int opcao;

printf("DIGITE O PRIMEIRO VALOR:");
scanf("%f", &valor1);
printf("DIGITE O SEGUNDO VALOR:");
scanf("%f", &valor2);

printf("\n BOA TARDE!! ESCOLHA UMA OPÇÃO:");
printf("\n 1-SOMAR");
printf("\n 2-SUBTRAIR");
printf("\n 3-DIVIDIR");
printf("\n 4-MULTIPLICAR");
scanf("%d", &opcao);

switch(opcao){
case 1: printf("RESULTADO DA SOMA: %.2f", valor1+valor2);
        break;
case 2:
    printf("RESULTADO DA SUBTRAÇÃO: %.2f", valor1-valor2);
    break;
case 3:
    printf("RESULTADO DA DIVISÃO: %.2f", valor1/valor2);
    break;
case 4:
    printf("RESULTADO DA MULTIPLICAÇÃO: %.2f", valor1*valor2);
    break;
default:
    printf("OPÇÃO INVÁLIDA");
    break;


}



}