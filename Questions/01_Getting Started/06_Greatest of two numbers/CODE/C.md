# Method 1 : Using if – else Statements

### Algorithm

The algorithm and the Explanation for the above problem is mentioned below.
For two numbers num1 & num2

*   If num1 == num2
    *   Print both are equal
*   Else if num1 > num2
    *   Print num1 is greater
*   Else, num2 has to be the greater
    *   Print num2 is greater

Let’s try and implement the algorithm in C Language.

## INPUT
```c
#include<stdio.h>

int main ()
{
  int num1, num2;
  num1=12,num2=13;

  if (num1 == num2)
    printf("both are equal");
  else if (num1 > num2) 
    printf("%d is greater", num1);
  else
    printf("%d is greater", num2);

  return 0;
}
```
## OUTPUT
```
13 is greater
```

# Method 2 : Using Ternary Operator

### Algorithm

In this method, we’ll use the knowledge of Ternary Operator in C . The Algorithm for the above mentioned problem is given below.
For two numbers num1 & num2

*   If num1 == num2
    *   Print both are equal
*   Else, use ternary operator (temp = num1 > num2? num1: num2)
    *   Print temp value is greater

Let’s try and implement the above algorithm in C Language.

## INPUT
```c
#include <stdio.h>
int main ()
{
    int num1, num2, temp;
    
    num1=20,num2=30;
    if(num1 == num2)
        printf("Both are Equal\n");
    else{
        temp = num1 > num2? num1 : num2;
        printf("%d is largest",temp);
    }

  return 0;
}
```
## OUTPUT
```
30 is greater
```
