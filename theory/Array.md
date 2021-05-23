# Digit Saperator
```c++
#include<stdio.h>
int main()
{
int password;
printf("Enter your password");
scanf("%d",&password);
int password_Array[5];
int i=0;
int mod =0;
for(i=0;i<5;i++){
    password_Array[i]= password%10;
    mod = password/10;
    password = mod;
}
 printf("Your pasword is\n");
for(i=4;i>=0;i--){
   printf("%d\n",password_Array[i]);
}
}
```
# Multiplication table Program
```C++
#include <stdio.h>
int main()
{
    int n;
    printf("Please enter the digit");
    scanf("%d", &n);
    int i;
    for (i = 1; i <= 10; i++)
    {
        printf("%d X %d = %d\n", n, i, (n * i));
    }
}
```
# Power of Any Number
```C++
#include <stdio.h>
#include <math.h>
int main()
{
    int x;
    printf("enter the number\n");
    scanf("%d", &x);
    int p;
    printf("Enter the Power");
    scanf("%d", &p);
    int power_of_x = pow(x, p);
    printf("Your answer is %d", power_of_x);
}
```
# PALINDROME CHECKER
```c++
#include <stdio.h>
int main()
{
    int num, r, sum = 0, t;
    printf("ENTER A NUMBER-\n");
    scanf("%d", &num);
    for (t = num; num != 0; num = num / 10)
    {
        r = num % 10;
        sum = sum * 10 + r;
    }
    if (t == sum)
        printf("%d is a palindrome number.\n", t);
    else
        printf("%d is not a palindrome number.\n", t);
}
```