# Method 1: Using if-else Statements

## INPUT
```cpp
#include 
using namespace std;

int main ()
{
    int num1, num2;
    num1=75,num2=85;
 
    if (num1 == num2)
        cout << "both are equal"; else if (num1 > num2)
        cout << num1 << " is greater than " << num2;
    else
        cout << num2 << " is greater than " << num1;

    return 0;
}

// Time Complexity : O(1)
// Space Complexity : O(1)
```
## OUTPUT
```
85 is greater than 75
```

### Working

For two user inputs num1 and num2.

*   Step 1: Check if both numbers are equal
    *   If true then print “Both are equal”
*   Step 2: Else if num1 > num2
    *   If true then print num1 greater than num2
*   Step 3: Else num2 has to be thee greatest
    *   Print num2 is greater than num1

# Method 2: Using Ternary Operator

## INPUT
```cpp
#include<bits/stdc++.h>
using namespace std;

int main ()
{
    int num1, num2, largest;
    num1=32,num2=47; 
 
    if(num1 == num2)
        cout << "Both are Equal\n"; else { largest = num1 > num2? num1 : num2;
        cout << largest << " is largest";
    }

  return 0;
}

// Time Complexity : O(1)
// Space Complexity : O(1)
```
## OUTPUT
```
47 is largest
```

### Working

This method uses knowledge of ternary operator in C++

For two user inputs num1 and num2.

*   Step 1: Check if both numbers are equal
    *   If true then print “Both are equal”
*   Step 2: Use ternary operator as largest = num1 > num2? num1 : num2;
*   Step 3: Print the value of variable largest

# Method 3: Using inbuilt max() Function

## INPUT
```cpp
#include <iostream>  
// function max available in here
#include <math.h>
using namespace std;

int main ()
{
    int num1, num2;
    num1=45,num2=14;
 
    if (num1 == num2)
        cout << "both are equal";
    else
        cout << max(num1,num2) << " is greater";

    return 0;
}

// Time Complexity : O(1)
// Space Complexity : O(1)
```
## OUTPUT
```
45 is greater
```

### Working

This method uses internal inbuilt function max(a, b) which returns the larger value.

For two user inputs num1 and num2.

*   Step 1: Check if both numbers are equal
    *   If true then print “Both are equal”
*   Step 2: Use inbuilt function max as max(num1, num2)
*   Step 3: Print the value of returned by max function

# Method 4: Using Classes

This method uses classes and objects concept in C++

## INPUT
```cpp
#include <iostream> 
using namespace std;

class PrepInsta
{
    public:
        int calcLargest(int, int);
};

int PrepInsta::calcLargest(int a, int b)
{
    if(a>b)
        return a;
    else
        return b;
}

int main()
{
    PrepInsta obj;
    int num1, num2, largest;
    
    num1=36,num2=23;
    
    largest = obj.calcLargest(num1, num2);
    cout<<"Largest: "<<largest;

    return 0;
}
```
## OUTPUT
```
Largest: 36
```