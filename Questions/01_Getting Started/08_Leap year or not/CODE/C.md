# Method 1 : Using if-else Statements 1

In this method we’ll use if-else statements to check for the required conditions for an Year to be a Leap Year.

### Working

For a given integer input as year, we do the following

*   Check if the year variable is divisible by 400. if true it’s a Leap Year, it’s not a Leap Year otherwise.
*   Check if the year variable is divisible by 4 and not by 100. If true, print it’s a Leap year, It’s not a Leap Year otherwise.

Let’s implement the above mentioned logic in C Language.

## INPUT
```c
#include <stdio.h>
int main ()
{
    int year;
    year=2000;
    
    if(year % 400 == 0)
        printf("%d is a Leap Year",year);
        
    else if(year % 4 == 0  && year % 100 != 0)
        printf("%d is a Leap Year",year);
        
    else
        printf("%d is not a Leap Year",year);
    
    return 0;
}
```
## OUTPUT
```
2000 is a Leap Year
```

# Method 2 : Using if-else Statements 2

In this method we’ll use if-else statements to check for the required conditions for an Year to be a Leap Year. This method is the simplified version of previous method.

### Working

For a Given integer input for an year, we check

*   If the year is divisible by 400. If true it’s a Leap Year, it’s not otherwise.
*   If the year is divisible by 4 and not by 100. It’s a leap year if true, it’s not otherwise.

Let’s implement the above logic in C Language.

## INPUT
```c
#include <stdio.h>
int main ()
{
    int year;
    year=2000;
    
    if(year % 400 == 0 || (year % 4 == 0  && year % 100 != 0))
        printf("%d is a Leap Year",year);
        
    else
        printf("%d is not a Leap Year",year);
    
    return 0;
}
```
## OUTPUT
```
2000 is a Leap Year
```