#  Temperature-Conversion-in-C
C language Temperature conversion program 

# include <stdio.h>
main()
{
	int x;
	printf("This are the temperature conversions available: ");
	printf("\n 1. for Celsuis");
	printf("\n 2. for Fahrenheit");
	printf("\n 3. for Kelvin");
	printf("\n 4. for Rankine");
	printf("\n Enter the temperature at which you are converting (1-4) : ");
	scanf("%d", &x);
	if (x == 1)
	{
	    int C;
	    float Fahrenheit, Kelvin, Rankine;
	    printf ("\n Enter your degree in Celsuis: ");
	    scanf ("%d", &C);
	    Fahrenheit = (C * 1.8) + (32);
	    Kelvin = C + 273.15; 
	    Rankine = (C * 1.8) + (32 + 459.67);
	    printf ("\n Fahrenheit = %f", Fahrenheit);
	    printf ("\n Kelvin = %f", Kelvin);
	    printf ("\n Rankine = %f", Rankine);
	}
	
	else if (x == 2)
	{
		int F; 
	    float Celsuis, Kelvin, Rankine;
	    printf("\n Enter your degree in Fahrenheit :");
	    scanf("%d", &F);
	    Celsuis = ((F - 32) / 1.8);
	    Kelvin = ((F + 459.67) / 1.8);
	    Rankine = (F + 459.67);
	    printf("\n Celsuis = %f", Celsuis);
	    printf("\n Kelvin = %f", Kelvin);
	    printf("\n Rankine = %f", Rankine);
	}	
	
	else if (x == 3)
	{
		int K; 
	    float Celsuis, Fahrenheit, Rankine;
	    printf ("\n Enter your degree in Kelvin: ");
	    scanf ("%d", &K); 
	    Celsuis = K - 273.15;
	    Fahrenheit = ((K * 1.8) - 459.67);
	    Rankine = K * 1.8;
	    printf("\n Celsuis = %f", Celsuis);
	    printf("\n Fahrenheit = %f", Fahrenheit);
	    printf("\n Rankine = %f", Rankine);
	}
	
	else if (x == 4)
	{
		int Ra; 
	    float Celsuis, Fahrenheit, Kelvin;
	    printf ("\n Enter your degree in Rankine: ");
	    scanf ("%d", &Ra);
	    Celsuis = ((Ra - 32 - 459.67) / 1.8);
	    Fahrenheit = Ra - 459.67;
	    Kelvin = Ra / 1.8;
	    printf("\n Celsuis = %f", Celsuis);
	    printf("\n Fahrenheit = %f", Fahrenheit);
	    printf("\n Kelvin = %f", Kelvin);
	}		
	
	else 
	    printf("\nInvalid Choice");
}
