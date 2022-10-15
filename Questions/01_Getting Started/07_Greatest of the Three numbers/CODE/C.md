# Method 1 : Using if-else Statements 1

## INPUT
```c
#include <stdio.h>
int main ()
{
    int num1, num2, num3;
    
    num1=13,num2=45,num3=27;

    //comparing num1 with other numbers
    if ((num1 >= num2) && (num1 >= num3))
        printf("%d is the greatest", num1);
        
    //comparing num2 with other numbers
    else if ((num2 >= num1) && (num2 >= num3))
         printf("%d is the greatest", num2);
    
    // num3 has to be greatest then if not above
    else
         printf("%d is the greatest", num3);
    
    return 0;
}
```
## OUTPUT
```
45 is the greatest
```

# Method 2 : Using if-else Statements 2

## INPUT
```c
#include <stdio.h>
int main ()
{
    int num1, num2, num3;
    
    num1=13,num2=45,num3=27;

    //comparing num1 with other numbers
    if ((num1 >= num2) && (num1 >= num3))
        printf("%d is the greatest", num1);
        
    //comparing num2 with other numbers
    else if ((num2 >= num1) && (num2 >= num3))
         printf("%d is the greatest", num2);
    
    // num3 has to be greatest then if not above
    else
         printf("%d is the greatest", num3);
    
    return 0;
}
```
## OUTPUT
```
45 is the greatest
```

# Method 3 : Using Ternary Operator

In this method we use the knowledge of Ternary Operators in C

> Ternary Operator Syntax: 
> ( Condition ) ? ( if True : Action ) : ( if False : Action )

## INPUT
```c
#include <stdio.h> 
int main ()
{
    int num1, num2, num3;
    
    num1=12,num2=98,num3=84;
    
    int temp, result;    
    
    // find the largest b/w num1 and num2 & store in temp
    temp = num1>num2 ? num1:num2;
    
    // find the largest b/w temp and num3 & finally printing it
    result = temp>num3 ? temp:num3;    
     
    printf(" %d is the largest", result);
    return 0;
}
```
## OUTPUT
```
98 is the largest
```