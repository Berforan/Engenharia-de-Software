# Engenharia-de-Software
Exercícios em c++
#include <iostream>
#include <locale.h>
using namespace std;
int main()
{
	setlocale(LC_ALL, "portuguese");
	int codigo, qtdade;
	float valor=0;
	char *item;
	
	cout <<"*** Cardápio ***\n";
	cout <<"100 - HAMBURGUER - R$5,50\n";
	cout <<"101 - CACHORRO-QUENTE - R$4,50\n";
	cout <<"102 - MILKSHAKE - R$10,50\n";
	cout <<"103 - PIZZA-40CM - R$40,00\n";
	cout <<"104 - X-TUDO - R$8,50\n";
	
	cout <<"informe o código do seu pedido: ";
	cin >>codigo;
	cout <<"informe a quantidade desejada: ";
	cin >>qtdade;
	switch (codigo)
	{
		case 100:
			item="HAMBURGUER";
			valor = qtdade * 5,50;
			break;
		
		case 101:
			item="CACHORRO-QUENTE";
			valor = qtdade * 4,50;
			break;
		
		case 102:
			item="MILKSHAKE";
			valor = qtdade * 10,50;
			break;
		
		case 103:
			item="PIZZA-40CM";
			valor = qtdade * 10,50;
			break;
		
		case 104:
			item="X-TUDO";
			valor = qtdade * 8,50;
			break;	
		
		default:
			cout <<"PEDIDO INVÁLIDO! ";
	}
	cout <<qtdade << " x " << item << " = " << valor;
	
}
