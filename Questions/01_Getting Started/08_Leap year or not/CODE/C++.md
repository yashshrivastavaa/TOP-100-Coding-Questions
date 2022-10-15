# Method 1: Using if-else Statements 1

In this method we’ll use the if-else statements to check for the above mentioned conditions one by one.

### Working

For user input year check

*   If year % 400 == 0
    *   Print Leap Year
*   Else If year % 4 == 0 && year % 100 != 0
    *   Print Leap Year
*   Else, year will be not leap

Let’s implement the above logic in C++ Language.

## INPUT
```cpp
#include <bits/stdc++.h>
using namespace std;

int main()
{
    int year;

    year=2000;

    if(year % 400 == 0)
        cout << year << " is a Leap Year";
        
    else if(year % 4 == 0  && year % 100 != 0)
        cout << year << " is a Leap Year";
        
    else
        cout << year << " is not a Leap Year";
    
    return 0;
}
```
## OUTPUT
```
2000 is a Leap Year
```

# Method 2: Using if-else Statements 2

In this method we’ll use the if-else statements to check for the above mentioned conditions one by one. This method is the more simplified version of the previous method.

### Working

For user input year check –

*   If (year % 400 == 0 || (year % 4 == 0 && year % 100 != 0))
    *   Print Leap Year
*   Else, year will be not leap

Let’s implement the above logic in C++ Language.

## INPUT
```cpp
#include<bits/stdc++.h>
using namespace std;
int main()
{
    int year;

    year=2000;

    if(year % 400 == 0 || (year % 4 == 0  && year % 100 != 0))
        cout << year << " is a Leap Year";

    //not leap year
    else
        cout << year << " is not a Leap Year";
    
    return 0;
}
```
## OUTPUT
```
2000 is a Leap Year
```

# Method 3: Using Ternary Operator 

In this method we’ll use the Ternary operator to check for the above mentioned conditions. For more information on Ternary operators check out Ternary operators in C.

### Working

For user input year check

*   Using ternary operator check if the year is divisible by 400. Print it’s a leap year.
*   Using Ternary operator check if the year is divisible by 4 but not with 100. Print it’s a leap year.
*   Else print it’s not a leap year.

Let’s implement the above mentioned logic in C++ Language.

## INPUT
```cpp
#include 
using namespace std;

int main()
{
    int year;
    year=2000;
    int flag = (year%400 == 0) || (year%4==0 && year%100!=0 ) ? 1 : 0;
    if (flag ==1)
    {
        printf("%d is a Leap Year",year);
    }
    else
    {
        printf("%d is not a Leap Year",year);
    }

    return 0;
}
```
## OUTPUT
```
2000 is a Leap Year
```

# Method 4: Complicated if-else statements

Some websites have also mentioned the below program as well, which is we why are just showing you the below, however, this is complicated to understand and code also we do not recommend writing this program below –

## INPUT
```cpp
#include <iostream>
using namespace std;

int main() {

    int year;

    year=2000;
  
    if (year % 4 == 0) {
        if (year % 100 == 0) {
            if (year % 400 == 0) {
                cout << year << " is a Leap Year";
            }
            else {
                cout << year << " is not a Leap Year";
            }
        }
        else {
            cout << year << " is a Leap Year";
        }
    }
    else {
        cout << year << " is not a Leap Year";
    }
    return 0;
}
```
## OUTPUT
```
2000 is a Leap Year
```