# ecuacion-de-la-recta
/En este programa se hara uso de estructuras para realizar la ecuacion de la recta dado dos puntos/
/Clase 15 de febrero___ALSE/
/Paula Andrea  Melo --- Christian Lara --- Daniel Rodruiguez/

#include <stdio.h>
#include <math.h>


struct punto 
{
	float x;
	float y;
};

int main ()
{
	/Teniendo la ecuacion punto pendiente------> Y-Y1=m(X-X1)/
	float pend,b; /Pend= pendiente entre los puntos/
	struct punto P1; /Primer punto dado/
	struct punto P2;  /Segundo punto dado/ 
	printf ("\tHola\n En este programa se podra obtener la ecuacion punto-pendiente \n");
	printf ("ingrese la coordenada en X del primer punto\n\t");  
	scanf ("%f",&P1.x); /Ingresa un X1______Se pone %f por ser flotante/
	printf ("ingrese la coordenada en Y del primer punto\n\t");
	scanf ("%f",&P1.y); /Ingresa un Y1/
	printf("ingrese la coordenada en X del segundo  punto\n\t"); 
	scanf ("%f",&P2.x);
	printf ("ingrese la coordenada en Y del segundo punto\n\t");
	scanf ("%f",&P2.y);
	pend= (P2.y-P1.y)/(P2.x-P1.x);/Ecuacion de pendiente (Y2-Y1)/(X2-X1)/
	b=(P1.y)+(pend*(-(P1.x))); /El intercepto se hace despejando de la ecuacion de tal forma que queda b=Y1+m(-X1)/
	printf("La ecuacion de la recta es:\n\t Y= %fX+ %f\n\n", pend, b); 									
}
