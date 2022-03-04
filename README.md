#include<stdio.h>

int main ()

{

int altura, i, estrela, aux, aux1, espaco;

estrela=1;

printf("n = ");
scanf ("%d", &altura);//entrada do tamanho da escada

espaco=altura;//igualando o tanto de espaços que vai ter a altura

for (i=1; i<=altura; i++)//for para montar a escada
{
    for(aux=espaco; aux>1; aux--)//for para a quantidade de " "
    {
        printf (" ");//enquanto o aux for maior que 1 vai imprimir " "
    }

    for(aux1=estrela; aux1>=1; aux1--)//for para a quantidade de "*"
    {
        printf ("*");//enquanto o aux1 for maior/igual a 1 vai imprimir "*"
    }

	estrela++;//vai aumentando o valor para aumentar a quantidade de "*" impressas até se igualar a altura 
	espaco--;//vai diminuido o valor para diminuir a quantidade de " " impressos até que na última linha 
	       //não tenha espaço

    printf ("\n");//um entender toda vez que terminar os for da "*" e " " para montar a escada

	}
	
return 0;

}
