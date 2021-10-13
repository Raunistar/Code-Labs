# LEAP YEAR CHECKER
```C
#include<stdio.h>

int main() {
    int num;
    printf("Enter an integer: ");
    scanf("%d", &num);
    if(num % 2 == 0){
        printf("%d is even.", num);
    }
    else{
        printf("%d is odd.", num);
    }
    return 0;
}
```
# POSITIVE OR NEGATIVE CHECKER
```c
#include <stdio.h>
int main()
{
    int num;
    printf("ENTER THE NUMBER::");
    scanf("%d", &num);
    if (num >= 0)
        printf("%d Number is positive", num);
    else
        printf("%d is negetive number", num);
}
```
# GREATEST OF THREE NUMBERS
```c
#include <stdio.h>
int main()
{
    int x, y, z;
    printf("ENTER three NUMBERS respectively::\n");
    scanf("%d%d%d", &x, &y, &z);
    if (x > y && x > z)

    {
        printf("%d is Largest", x);
    }

    if (y > x && y > z)
    {
        printf("%d is Largest", y);
    }
    if (z > x && z > y)

        printf("%d is LARGEST", z);
}
```
# VOWEL AND CONSONANT CHECKER 
```c
#include <stdio.h>
int main()
{
    char c;
    printf("ENTER AN ALPHABET::");
    scanf("%c", &c);
    if (c == 'a' || c == 'e' || c == 'i' || c == 'o' || c == 'u' || c == 'A' || c == 'I' || c == 'E' || c == 'O' || c == 'U')

    {
        printf("ITS A VOWEL");
    }
    else
        printf("ITS A CONSONANT");

    return 0;
}
```
# ASCII VALUE OF A CHARACTER
```c
#include <stdio.h>
int main()
{
    char c;
    printf("ENTER A CHARACTER::");
    scanf("%c", &c);
    printf("ASCII value =%d", c);
    return 0;
}
```
# QUOTEINT AND REMAINDER FINDER
```c
#include <stdio.h>
int main()
{
    int D, d, Q, R;
    printf("ENTER the dividend ::");
    scanf("%d", &D);
    printf("ENTER the divisor::");
    scanf("%d", &d);

    Q = D / d;
    R = D % d;

    printf("QUOTEINT = %d", Q);
    printf("\n REMAINDER = %d", R);
}
```
# SWAPPING OF TWO NUMBERS USING THIRD VARIABLE
```c
#include <stdio.h>
int main()
{
    int x, y, temp;
    printf("ENTER x :: ");
    scanf("%d", &x);
    printf("ENTER y :: ");
    scanf("%d", &y);

    temp = x;
    x = y;
    y = temp;
    printf("AFTER SWAPPING");
    printf("\n x=%d", x);
    printf("\n y=%d", y);
}
```
# SUM AND AVERAGE FOR SOME NUMBERS
```c
#include <stdio.h>
int main()
{
    int i, x, sum = 0;
    float avg;
    printf("ENTER the 5 NUMBERS :: \n");
    for (i = 1; i <= 5; i++)
    {
        printf("NUM-%d :: ", i);
        scanf("%d", &x);
        sum += x;
    }
    avg = sum / 5.0;
    printf("THE sum of 5 no is :: %d", sum);
    printf("\n THE avg. is :: %f\n", avg);
}
```
# FACTORIAL OF GIVEN NUMBER
```c
#include <stdio.h>
int main()
{
    int i, f = 1, x;
    printf("ENTER THE NUMBERS :: ");
    scanf("%d", &x);

    for (i = 1; i <= x; i++)
        f = f * i;
    {
        printf("THE FACTORIAL OF %d is :: %d\n", x, f);
    }
}
```
# MAX AMONG THREE NUMBERS
```c
#include <stdio.h>
int main()
{
    int a, b, c, max;
    printf("enter the 1st num :");
    scanf("%d", &a);
    printf("enter the 2nd num :");
    scanf("%d", &b);
    printf("enter the 3rd num :");
    scanf("%d", &c);
    if (a > b && a > c)
    {
        max = a;
    }

    else if (b > a && b > c)
    {
        max = b;
    }
    else if (c > a && c > b)
    {
        max = c;
    }
    printf("Max among all is:%d");
}
```
# DISTANCE BETWEEN TWO POINTS
```c
#include <stdio.h>
#include <math.h>
int main()
{
    int x1, y1, x2, y2;
    float dist;
    printf("x1 is :");
    scanf("%d", &x1);
    printf("x2 is :");
    scanf("%d", &x2);
    printf("y1 is :");
    scanf("%d", &y1);
    printf("y2 is :");
    scanf("%d", &y2);
    dist = (x2 - x1) * (x2 - x1) + (y2 - y1) * (y2 - y1);
    printf("the distance beween two point is =%.4f", sqrt(dist));
}
```
# PALINDROME CHECKER
```c
#include <stdio.h>
int main()
{
    int r, num, t, sum = 0;
    printf("ENTER a number :: ");
    scanf("%d", &num);

    for (t = num; num != 0; num = num / 10)
    {
        r = num % 10;
        sum = sum * 10 + r;
    }
    if (t == sum)
    {
        printf("%d IS A PALINDROME NO \n", t);
    }
    else
        printf("%d is not a PALINDROME no \n", t);
}
```
# ALL NATURAL NUMBERS IN REVERSE
```c
#include <stdio.h>
int main()
{
    int n;
    printf("ENTER value of n :: ");
    scanf("%d", &n);

    while (n >= 1)
    {
        printf("%d\n", n);
        n--;
    }
}
```
# USE OF STRING COPY
```c
#include <stdio.h> // needed for printf
#include <string.h> // needed for strcpy
int main() {
 char name[50];
 strcpy(name, "Alice in Wonderland");
 printf("Hello, %s\n", name);
}
```
# calculate interest and service charge for bank customer
```c
//calculate interest and service charge for bank customer
#include <stdio.h>
int main()
{
    char customer[30], acctNum[30];
    double avgBalance, interest, service;
    int numTrans;
    printf("Name? ");
    gets(customer);
    printf("Account number? ");
    gets(acctNum);
    printf("Average balance? ");
    scanf("%lf", &avgBalance);
    printf("Number of transactions? ");
    scanf("%d", &numTrans);
    interest = avgBalance * 0.06;
    service = numTrans * 0.50;
    printf("\nName: %s\n", customer);
    printf("Average balance: $%3.2f\n", avgBalance);
    printf("Interest: $%3.2f\n", interest);
    printf("Service charge: $%3.2f\n", service);
}
```
# TICKET COLLECTION AND SOLD
```c

//calculate ticket sales for football match
#include <stdio.h>
int main() {
 double rPrice, sPrice, gPrice;
 double rSales, sSales, gSales, tSales;
 int rTickets, sTickets, gTickets, tTickets;
 printf("Reserved price and tickets sold? ");
 scanf("%lf %d", &rPrice, &rTickets);
 rSales = rPrice * rTickets;
 printf("Stands price and tickets sold? ");
 scanf("%lf %d", &sPrice, &sTickets);
 sSales = sPrice * sTickets;
 printf("Grounds price and tickets sold? ");
 scanf("%lf %d", &gPrice, &gTickets);
 gSales = gPrice * gTickets;
 tTickets = rTickets + sTickets + gTickets;
 tSales = rSales + sSales + gSales;
 printf("\nReserved sales: $%3.2f\n", rSales);
 printf("Stands sales: $%3.2f\n", sSales);
 printf("Grounds sales: $%3.2f\n", gSales);
 printf("\n%d tickets were sold\n", tTickets);
 printf("Total money collected: $%3.2f\n", tSales);
}
```
# JOB CHARGE BASED ON HOUR WORKED & COST OF PART
```c
//print job charge based on hours worked and cost of parts
#include <stdio.h>
int main() {
 double hours, parts, jobCharge;
 printf("Hours worked? ");
 scanf("%lf", &hours);
 printf("Cost of parts? ");
 scanf("%lf", &parts);
 jobCharge = hours * 100 + parts;
 if (jobCharge < 150) jobCharge = 150;
 printf("\nCharge for the job: $%3.2f\n", jobCharge);
}
```
# USE OF FUNCTION SKIPLINES
```c
#include <stdio.h>
int main()
{
    void skipLines(int);
    printf("Sing a song of sixpence\n");
    skipLines(2);
    printf("A pocket full of rye\n");
} //end main
void skipLines(int n)
{
    for (int h = 1; h <= n; h++)
        printf("\n");
} //end skipLines
```
# GETS (STR) USE
```c
#include <stdio.h>
int main()
{
    printf("\n\n\n\t\t WELCOME TO STARLAB\n\n\n");
    char str[50];
    printf("PLEASE ENTER YOUR NAME ::\n\n\n ");
    gets(str);
    printf("\n\n\nWELCOME TO STARLAB %s\n\n\n", str);
    return 0;
}
```
# USING FUNCTION FOR 1st TIME
```c
#include <stdio.h>
int addNum(int, int, int);
int main()
{
    int a, b, c, R;
    printf("ENTER THE NUMBERS::\n");
    scanf("%d%d%d", &a, &b, &c);
    R = addNum(a, b, c);

    printf("%d", R);
}
int addNum(int a, int b, int c)

{
    printf("THE FINAL VALUE IS :: ");
    int results = a + b + c;
}
```
# USING STRUCTURE FOR STUDENT DETAILS
```c
#include <stdio.h>
struct student
{
    char name[20];
    int id;
    char address[30];
    int phone_no;
};
int main()
{
    struct student std;
    printf("Enter Details :: \n");
    printf("student Name :: ");
    gets(std.name);
    printf("student id::");
    scanf("%d", &std.id);
    printf("student address:: ");
    scanf("%s", &std.address);
    printf("student phone_no::");
    scanf("%d", &std.phone_no);

    printf("Enter Details are:: \n");
    printf("\nstudent Name ::%s ", std.name);
    printf("\nstudent id::%d ", std.id);

    printf("\nstudent address::%s ", std.address);

    printf("\nstudent phone_no:: %d", std.phone_no);
}
```
# USING ARRAY OF STRUCTURE FOR STUDENT DETAILS
```c
#include <stdio.h>
struct student
{
    char firstName[50];
    char student;
    int id;
    char address[50];
    int phone_no;

} s[10];

int main()
{
    int i;
    printf("Enter Details of students:\n");

    // storing information
    for (i = 0; i < 5; ++i)
    {
        s[i].student = i + 1;
        printf("\nFor student  %d,\n", s[i].student);
        printf("Enter first name: ");
        scanf("%s", s[i].firstName);
        printf("Enter the student id:", s[i].id);
        scanf("%d", &s[i].id);
        printf("\nEnter the address:");
        scanf("%s", &s[i].address);
        printf("Enter the phone number:");
        scanf("%d", &s[i].phone_no);
    }
    printf("Displaying Information:\n\n");

    // displaying information
    for (i = 0; i < 5; ++i)
    {
        printf("\nstudent: %d\n", i + 1);
        printf("First name: ");
        puts(s[i].firstName);
        printf("Enter the student id:", s[i].id);
        printf("\naddress: %s", s[i].address);
        printf(" phone number:", s[i].phone_no);
        printf("\n");
    }
    return 0;
}
```
# STARLAB
```c
#include <stdio.h>
struct member
{
   char name[30];
   int id;
   int pass;
};
int main()
{
   printf("\n-------------------------------------\n");
   printf("\n-------welcome to STARLAB------------\n");
   struct member emp;
   printf("\n-----ENTER YOUR DETAILS HERE-----\n");
   printf("Name:: ");
   gets(emp.name);
   printf("id::");
   scanf("%d", &emp.id);
   printf("pass::");
   scanf("%d", &emp.pass);

   printf("\n----ENTER DETAILS ARE----\n");
   printf("your name is : %s\n", emp.name);
   printf("your entered id is : %d\n", emp.id);
   printf("you password is : %d\n", emp.pass);

   printf("\n---------ACCESS GRANTED-----------\n");
   printf("--------WELCOME TO STARLAB '%s'--------\n", emp.name);
}
```
# AVERAGE OF ARRAY ELEMENTS USING POINTER
```c
#include <stdio.h>
int main()
{
    float x[5], avg;
    int i;
    float *px, *pavg;
    px = &x[0];
    pavg = &avg;
    printf("Enter array Elements : ");
    for (i = 0; i < 5; i++)

    {
        scanf("%f", (px + i));
        *pavg += *(px + i) / 5;
    }
    printf("Average=%.2f\n", *pavg);
}
```

``` 
1 2 3 4
1 2 3 4
5 6 7 8

```
# POWER OF ANY NUMBER
```c
#include <stdio.h>
#include <math.h>
int main()
{
    int x, y, z;
    printf("The number & power is :\n");
    scanf("%d%d", &x, &z);

    y = pow(x, z);
    printf("The value is =%d\n", y);
}
```
# THE AVG OF TWO NUMBERS IN C++
```c++
#include <iostream>
using namespace std;
int main()
{
    float num1, num2, avg;
    cout << "Enter the num1 and num2::";
    cin >> num1;
    cin >> num2;
    float sum = num1 + num2;
    avg = sum / 2;
    cout << "the sum is =" << sum << "\n";
    cout << "The avg is =" << avg << "\n";
    return 0;
}
```
# LARGEST BETWEEN TWO NO'S IN C++
```c++
#include <iostream>
using namespace std;
int main()
{
     float num1, num2;
     cout << "num1=";
     cin >> num1;
     cout << "num2=";
     cin >> num2;
     if (num1 > num2)
     {
          cout << "num1 is largest :)";
     }
     if (num2 > num1)
     {
          cout << "num2 is largest :(";
     }
     return 0;
}
```
# FAHRENHEIT TO CELCIUS IN c++
```c++
#include <iostream>
using namespace std;
int main()
{
     float fahr, cels;
     cout << "Enter the temperature in fahrenhite=";
     cin >> fahr;
     cels = (fahr - 32) * 5 / 9;
     cout << "The temperature in celcius is =" << cels << "\n";
     return 0;
}
```
