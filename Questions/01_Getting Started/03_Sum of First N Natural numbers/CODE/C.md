# Method 1: Using Brute Force

This method simply checks if the given input integer is divisible by 2 or not. If it’s divisible then print Even or Odd otherwise.

## INPUT
```c
#include <stdio.h>

int main ()
{
    int number;
    printf ("Insert a number \n");
    scanf ("%d", &number);

    //Checking if the number is divisible by 2
    if (number % 2 == 0)
        printf ("Even");
    else
        printf ("Odd");
  
    return 0;
}
```
## OUTPUT
```
Insert a number
10
Even
```

### Algorithm

For a user input **num**

*   If number % 2 == 0
    *   If true then the number is even
    *   Else, the number has to odd

Here % is called as modulo/remainder operator

# Method 2: Using Ternary Operator

This Method uses the ternary operator to check if the integer input is divisible by 2, If true print Even or Odd otherwise.

## INPUT
```c
#include <stdio.h>
int main ()
{
    int number;
    printf ("Insert a number \n");
    scanf ("%d", &number);
    
    //Checking if the number is divisible by 2
    number % 2 == 0? printf ("Even"):printf ("Odd");
    
    return 0;
}
```
## OUTPUT
```
Insert a number
15
Odd
```

### Algorithm

*   If number % 2 == 0
    *   If true then the number is even
    *   Else, the number has to odd

Here % is called as modulo/remainder operator

# Method 3: Using Bitwise Operator

This Method uses bitwise operators to check if a given number is Even or Odd.

## INPUT
```c
#include <stdio.h> 

// Returns true if n is even, else odd
int isEven(int num)
{
    // num & 1 is 1, then odd, else even
    return (!(num & 1));
}
 
// Driver code
int main()
{
    int num;
    printf("Enter the number: ");
    scanf("%d",&num);

    isEven(num)? printf ("Even"):printf ("Odd");
 
    return 0;
}
```
## OUTPUT
```
Insert a number
5
Odd
```

### Algorithm

For this method, we use the bitwise operator, in this case, bitwise and (&) How this works is below

*   For any number following operation : (num & 1) will always result
    *   1: If num is odd
    *   0: if num is even

**Let’s see how**

```
// 5 (in binary) : 00000101 
// 1 (in binary) : 00000001

    0 0 0 0 0 1 0 1

  & 0 0 0 0 0 0 0 1

  - - - - - - - - -

    0 0 0 0 0 0 0 1 
```