SUNIL MEENA (IOT620)
PROJECT 35@IOT
TASK ID = 150
C Program for convert Temperature Celsius to Fahrenheit →
#include <stdio.h>
float convertCtoF(float c)
{
 return ((c * 9.0 / 5.0) + 32.0);
}
int main()
{
 float c, f;
 printf("Enter temperature in Celsius: ");
 scanf("%f", &c);
 
 f = convertCtoF(c);
 printf("%.2f Celsius = %.2f Fahrenheit", c, f);
 return 0;
}
C Program for convert Temperature Fahrenheit to Celsius →
#include <stdio.h>
float convertFtoC(float f)
{
 return ((f - 32) / 1.8);
}
int main ()
{
 float c, f;
 printf ("\n\nEnter temperature in Fahrenheit: ");
 scanf ("%f”, &f);
 c = convertFtoC(f);
 printf ("%.2f Fahrenheit = %.2f Celsius", f, c);
 return 0;
}
Currency Conversion →
#include <stdio.h>
int main()
{
 float amount;
 float INR, USD, AED;
 int choice;
 printf ("Following are the Choices:");
 printf ("\nEnter 1 to convert INR to USD and AED: INR");
 printf ("\nEnter 2 to convert USD to INR and AED: USD");
 printf ("\nEnter 3 to convert AED to INR and USD: AED");
 printf ("\nEnter your choice: ");
 scanf ("%d", &choice);
 printf ("Enter the amount you want to convert?\n");
 scanf("%f", &amount);
 switch (choice)
 {
 case 1:
 printf("%.2f INR = %.2f USD", amount, amount*0.013);
 printf("\n%.2f INR = %.2f AED", amount, amount*0.047);
 break;
 case 2: 
 printf("\n%.2f USD = %.2f INR", amount, amount*77.69);
 printf("\n%.2f USD = %.2f AED", amount, amount*3.67);
 break;
 case 3:
 
 printf ("\n%.2f AED = %.2f INR", amount, amount*21.15);
 printf ("\n%.2f AED = %.2f USD", amount, amount*0.27);
 break;
 default:
 printf("\nInvalid Input");
 }
 return 0;
}
Number conversion
 Binary to Hexadecimal →
#include <stdio.h>
int main ()
{
 long int bi, hex = 0, i = 1, m;
 printf ("Enter the binary number: ");
 scanf ("%ld", &bi);
 while (bi != 0)
 {
 m = bi % 10;
 hex = hex + m * i;
 i = i * 2;
 bi = bi / 10;
 }
 printf ("Equivalent hexadecimal value: %lX", hex);
 return 0;
}
Binary to Decimal →
#include <stdio.h>
#include <math.h>
int main () {
 long long n;
 printf ("Enter a binary number: ");
 scanf ("%lld", &n);
 printf ("%lld in binary = %d in decimal", n, convert(n));
 return 0;
}
int convert(long long n) {
 int dec = 0, i = 0, m;
 while (n!=0) {
 m = n % 10;
 n /= 10;
 dec += m * pow (2, i);
 ++i;
 }
 return dec;
}
Hexadecimal to Binary →
#include<stdio.h>
int main ()
{
 char hexNum[100];
long int count=0;
printf ("Enter a hexadecimal number To Convert it into Binary: ");
scanf ("%s”, hexNum);
print f("\n Binary Number is : ");
while(hexNum[count])
{
switch(hexNum[count])
{
case '0' : printf ("0000");
break;
case '1' : printf("0001");
break;
case '2' : printf("0010");
break;
case '3' : printf("0011");
break;
case '4' : printf("0100");
break;
case '5' : printf("0101");
break;
case '6' : printf("0110");
break;
case '7' : printf("0111");
break;
case '8' : printf("1000");
break;
case '9' : printf("1001");
break;
case 'A' : printf("1010");
break;
case 'B' : printf("1011");
break;
case 'C' : printf("1100");
break;
case 'D' : printf("1101");
break;
case 'E' : printf("1110");
break;
case 'F' : printf("1111");
break;
case 'a' : printf("1010");
break;
case 'b' : printf("1011");
break;
case 'c' : printf("1100");
break;
case 'd' : printf("1101");
break;
case 'e' : printf("1110");
break;
case 'f' : printf("1111");
break;
default : printf("\nInvalid Entry, Please Try Again %c",hexNum[count]);
}
count++;
}
return 0;
}
Decimal to Binary →
#include <stdio.h>
int main ()
{
 int a[10], number, i, j;
 printf("\n Please Enter the Number You want to Convert : ");
 scanf("%d", &number);
 
 for(i = 0; number > 0; i++)
 {
 a[i] = number % 2;
 number = number / 2;
 }
 
 printf ("\n Binary Number of a Given Number = ");
 for(j = i - 1; j >= 0; j--) {
 printf(" %d ", a[j]);
 }
 printf("\n");
 return 0;
}
