[main (1).c](https://github.com/user-attachments/files/22139605/main.1.c)[Uploading main /******************************************************************************

                            Online C Compiler.
                Code, Compile, Run and Debug C program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

#include <math.h>
#include <stdio.h>
int main()
{ float desc, Vl_unitario, Qde, Vl_total,Vl_exced, Vl_unitario_desc;

	printf("Digite o valor unitario: ");
	scanf("%f",&Vl_unitario);
	
	printf("Digite o valor de desconto em %%: ");
	scanf("%f",&desc);
	desc = desc/100;
	
	Vl_unitario_desc = Vl_unitario - (Vl_unitario * desc);
	printf("Digite a qde de botton vendida: ");
	scanf("%f",&Qde);
	if (Qde < 101)
	 Vl_total = 100 * Vl_unitario;
	 
	else
	{
	Vl_exced = Qde - 100;
	Vl_total = 100 * Vl_unitario + Vl_exced * Vl_unitario_desc;
	}
	
	printf("\nValor total; %.2f\n ", Vl_total);
	return 0;
}
(1).c…]()
