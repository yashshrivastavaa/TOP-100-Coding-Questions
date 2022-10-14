# Method 1 : Using Brute Force

## INPUT
```c
#include <stdio.h>

int main()
{
    int a = 5;
    int b = 10;
    
    int sum = 0;
    
    for (int i = a; i <= b; i++)
        sum = sum + i;
    
    printf("%d",sum);
    
    return 0;
}
// Time complexity : O(N)
// Space complexity : O(1)
```
## OUTPUT
```
45
```

### Algorithm

The algorithm and working of the above mentioned problem is mentioned below,

*   Include the required Header files using include keyword.
*   Initialize the required variables.
*   Create a variable sum = 0
*   Run for loop in iterations of (I) in between [a, b]
    *   In each iteration add I to sum value
    *   Print sum value

Now let’s try and implement the algorithm in C language.

# Method 2 : Using the Formula

## INPUT
```c
#include <stdio.h>

int main()
{
    int a = 5;
    int b = 10;
    
    int sum = b*(b+1)/2 - a*(a+1)/2 + a;
    
    printf("%d",sum);
    
    return 0;
}
// Time complexity : O(1)
// Space complexity : O(1)
```
## OUTPUT
```
45
```

### Algorithm

This method uses a concept that the sum of first n natural numbers can be found using direct formulae – **n(n+1)/2**

For sum between [a, b] we can simply –

*   Create a variable sum = 0
*   sum = b*(b+1)/2 – a*(a+1)/2 + a
*   Print the sum

**Note** – An extra ‘a’ is added at the end for offset (check last part of the formula)

**Example** – Assume you had to calculate sum b/w [3, 5]. Doing b*(b+1)/2 – a*(a+1)/2 what we have done is subtracted (1, 2, 3) from (1, 2, 3, 4, 5). Thus only got the sum of (4, 5). So extra 3 i.e. a is added in the formula

# Method 3 : Using Recursion

## INPUT
```c
#include <stdio.h>

int getSum(int sum, int i, int b){
        
    // stop when any recursion call tries to go over b (larger number)
    if (i > b)
        return sum;

    return i + getSum(sum, i + 1, b);
}

int main()
{
    int a = 5;
    int b = 10;
    
    int sum = getSum(0, a, b);
    
    printf("%d",sum);
    
    return 0;
}
// Time complexity : O(N)
// Space complexity : O(1)
// Auxilary Space complexity : O(1)
// Because of function call stack
```
## OUTPUT
```
45
```

### Algorithm

Uses recursion starting with a (lower number) but only going till b (upper number)

For sum between [a, b] we can simply –

*   Include the Required header files using include keyword.
*   Initialize the required variables.
*   Create a variable sum = 0
*   Call function getSum(0, a, b)  
    *   In each recursion, call return i + getSum(sum, i + 1, b)
    *   In base Case i.e. when recursion call goes beyond upper limit return sum

Let’s try and implement the above algorithm in C Language.