# Method 1: Using for Loop

In this method we’ll add all the natural numbers until the given integer input using for loop in C++.

## INPUT
```cpp
#include<bits/stdc++.h> 
using namespace std;

int main()
{
    int n;
    cout << "Enter a number : "; 
    cin >> n;
    
    int sum=0;
    
    for(int i=1;i<=n;i++) 
        sum+=i;

    cout << sum;

    return 0;
}
```
## OUTPUT
```
Enter a number : 10
55
```

### Working

For a user input num.

*   Initialize a variable sum = 0.
*   Using a for loop in iteration ‘i’ iterate between [1, num].
*   Each time add ‘i’ to current sum as sum = sum + i.
*   Print sum.

### Explanation

Given an integer input N, the objective is to calculate the sum of all the natural numbers until the integer N. To do so we iterate through all the numbers that lay within N and keep incrementing the sum value.

The algorithm for the above code is as follows,

*   Include the required header files using the include keyword.
*   In the main() function initialize the required variables.
*   Run a for loop with range as N+1.
*   Keep adding the iter values to the Sum variable.
*   Print Sum variable using cout keyword.

The output for the above mentioned code is the sum of all the natural numbers until the given value.

# Method 2: Using Formula for the Sum of Nth Term

In this Method we use the formula for finding the sum of N term.

> Formula to Find the Sum of N terms: 
> Sum = ( Num * ( Num + 1 ) ) / 2

## INPUT
```cpp
#include<bits/stdc++.h>
using namespace std;

int main()
{
    int n;
    
    cout << "Enter a number : "; 
    cin >> n;
    
    cout << n*(n+1)/2;
    
    return 0;
}
```
## OUTPUT
```
Enter a number : 10
55
```

### Working

For a user input n.

*   Step 1: Initialize a variable sum = 0.
*   Step 2: Use formula sum = n(n+1)/2
*   Step 3: Print sum

### Explanation

Given an integer input N, the objective is to calculate the sum of all the natural numbers until the integer N. To do so we iterate through all the numbers that lay within N and keep incrementing the sum value.

The algorithm for the above code is as follows,

*   Include the required header files using the include keyword.
*   In the main() function initialize the required variables.
*   Run a for loop with range as N+1.
*   Keep adding the iter values to the Sum variable.
*   Print Sum variable using cout keyword.

This algorithm uses the formula n(n+1)/2 that can be used to find sum of first N natural numbers. This also reduces the time complexity from O(n) to O(1). The output for the above mentioned code is the sum of all the natural numbers until the given value.

# Method 3: Using Recursion

This method uses Recursion to recursively add the natural numbers up to the given integer input using recursion in c++.

## INPUT
```cpp
#include<bits/stdc++.h>
using namespace std;

int getSum(int n)
{
    if(n==0) 
        return n;
        
    return n + getSum(n-1);
}

int main()
{
    int n;
    cout << "Enter a number : "; 
    cin >> n;
    
    int sum = getSum(n);
    
    cout << sum;
    
    return 0;
}
```
## OUTPUT
```
Enter a number : 10
55
```

### Working
*   
For a user input n.

*   Initialize a variable sum = 0.
*   Call function getSum (n).
*   In each recursive call add the current value of n and call for lower recursion call using return n + getSum(n-1);
*   Print sum value

### Explanation

Given an integer input N, the objective is to calculate the sum of all the natural numbers until the integer N. To do so we recursively call a function  iterate through all the numbers that lay within N and keep incrementing the sum value.

The algorithm for the above code is as follows,

*   Include the required header files using the include keyword.
*   Define a Recursive function getSum() which takes the number input as an argument.
*   Recursively call the function and keep on adding the return statements.
*   In the main() function initialize the required variables.
*   Call the Recursive function and print out the returned value using cout keyword.

The output for the above mentioned code is the sum of all the natural numbers until the given value.