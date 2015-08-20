#include "stdafx.h"
#include "conio.h"
#include <iostream> 
#include <stdlib.h>
 
using namespace std;
void main()


	{int N, salariominimo=1400, i;
	
		float salariobruto,salarioneto, suma, promedio;
		cout<<"ingrese el numero de trabajadores";
		cin>>N;
		suma=0;

		for (i=0;i<N;i++)
		{
			cout<<"ingrese el salario bruto del trabajador:";
			cin>>salariobruto;
			if (salariobruto>(2*salariominimo))
			{salarioneto=salariobruto-(salariobruto*0.121)-(salariobruto*0.13);
			}
			else
			{salarioneto=salariobruto-(salariobruto*0.121);
			}
			suma=suma+salarioneto;
		}
		promedio=suma/N;
		cout<<"el promedio de los sueldos netos es:"<<promedio;
		getch();
	}

