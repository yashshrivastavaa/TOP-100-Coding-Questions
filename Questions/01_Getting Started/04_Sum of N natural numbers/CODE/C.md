# Method 1: Iterative way

## INPUT
```c
#include <stdio.h>

int main()
{
    int n; 
    scanf("%d",&n);
    
    int sum = 0;
    
    for(int i=1;i<=n;i++) 
        // is same as writing sum = sum + i
        sum += i;
        
    printf("Sum is %d",sum);
    
    return 0;
}

// Time complexity : O(n)
// Space complexity : O(1)
```
## OUTPUT
```
5
Sum is 15
```

### Algorithm

For an input n

*   Create variable sum = 0
*   Run a for loop in iteration (I) from 1 -> n
    *   Each time adding I to sum
*   Print the sum value after the loop terminates

# Method 2: Using Ternary Operator

This Method uses the ternary operator to check if the integer input is divisible by 2, If true print Even or Odd otherwise.

## INPUT
```c
#include <stdio.h>

int main()
{
    int n; 
    scanf("%d",&n);
    
    int sum = n*(n+1)/2;

    printf("The sum is %d",sum);
    
    return 0;
}
// Time complexity : O(1)
// Space complexity : O(1)
```
## OUTPUT
```
6
Sum is 21
```

### Algorithm

For an input n

*   Create variable sum = 0
*   Use formula sum =  n(n+1)/2
*   Print the sum value

# Method 3: Using Bitwise Operator

This Method uses bitwise operators to check if a given number is Even or Odd.

## INPUT
```c
#include <stdio.h>

int getSum(int sum,int n)
{
    if(n==0) 
        return sum;
        
    return n+getSum(sum,n-1);
}

int main()
{
    int n, sum = 0; 
    scanf("%d",&n);

    printf("%d",getSum(sum, n));
    
    return 0;
}
// Time complexity : O(n)
// Space complexity : O(1)
// Auxilary space complexity : O(N)
// Due to function call stack
```
## OUTPUT
```
5
Sum is 15
```

### Algorithm

For an input n

*   Create variable sum = 0
*   Call function getSum(sum, n)
    *   Base Case, n == 0 return sum
    *   Others return n + getSum(sum, n-1)
*   Print the sum value in main