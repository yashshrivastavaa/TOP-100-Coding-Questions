# Method 1: Using Brute Force

This method uses Brute Force to check whether a given integer is Positive or Negative.

## INPUT
```cpp
#include <iostream>
using namespace std;

int main()
{
    int num = 96;
    
    //Conditions to check if the number is negative or positive
    if (num > 0)
         cout << "The number is positive";
    else if (num < 0)
        cout << "The number is negative";
    else
        cout << "Zero";
    
    return 0;
}
```
## OUTPUT
```
Enter a number: 96
The number is Positive
```

### Algorithm

This method uses Brute Force to check whether a given integer is Positive or Negative. The Algorithm for the above code is as follows

*   Step 1. Start
*   Step 2. Insert the number.
*   Step 3. If the number is greater than Zero then print “The number is Positive”
*   Step4: If the number is smaller than zero, then print, “The number is Negative”
*   Step 5. Else print, “The number is Zero”
*   Step 6. Stop

# Method 2: Using Nested if-else Statements

This method uses a nested if-else Statements to check whether a given number is Positive or Negative.

## INPUT
```cpp
#include<iostream>
using namespace std;

int main()
{
    int num = -12;
    
    //Condition to check if the number is negative or positive
    if (num >= 0)
    {
        if (num == 0)
            cout << "Zero";
        else
            cout << "The number is positive";
    }
    else
            cout << "The number is negative";
    
    return 0;
}
```
## OUTPUT
```
Enter a number: -12
The number is Negative
```

### Algorithm

This method uses a nested if-else Statements to check whether a given number is Positive or Negative.

*   Step 1 – Start
*   Step 2 – Insert the number.
*   Step 3 – If the number is greater or equal move to the inner nested loop
    *   Step 3.1 – If the number is zero, print Zero
    *   Step 3.2 – Else print The Number is Positive
*   Step 4 – Else the number has to be negative, Print The number is Negative
*   Step 5 – Stop

# Method 3: Using Ternary Operator

This method uses a ternary operator to check whether a number is Positive or Negative.

> Ternary Operator Syntax: 
> ( Condition ) ? ( if True : Action) : ( if False : Action) ;

## INPUT
```cpp
#include <iostream>
using namespace std;

int main()
{
    int num = -15;
    
    //Condition to check if the 0, positive or negative
    
    if(num == 0)
            cout << "Zero"; else (num > 0) ? cout << "Positive": cout << "Negative";
    
    return 0;
}
```
## OUTPUT
```
Enter a number: -15
Negative
```

### Algorithm

This method uses a ternary operator to check whether a number is Positive or Negative. The Algorithm for the above code is as follows,
 
*   Step 1 – Start
*   Step 2 – Insert the number.
*   Step 3 – If number is equal to zero, Print Number is Zero
*   Step 4 – Else do following – (num > 0) ? cout << “Positive”: cout << “Negative”;
*   Step 5 – Stop