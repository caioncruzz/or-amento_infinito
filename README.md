# include <stdio.h>
# include <stdlib.h>
# include <locale.h>

int main () {
	
	setlocale (LC_ALL, "Portuguese");
	int salario,perda,Mperda,total;
	
	printf("Quanto e o seu salário:\n");
	scanf("%d",&salario);
	
	do{
		
		printf("Quanto você gastou:\n");
		scanf("%d",&Mperda);
		if (Mperda > 0)
		{
			
			total += Mperda;
			
		}
		
	}while(Mperda > 0);
	
	
	printf("O total de gastos foi: %d\n\n",total);
	
	if(total <= salario)

		printf("Gastos dentro do orçamento\n");
		
	else

			printf("Orçamento estourado\n");
	
	
	system("pause");
	
}
