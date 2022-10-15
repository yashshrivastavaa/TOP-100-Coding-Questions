# Method 1:

### Working

For user inputs of numbers as first, second and third.

*   Step 1: Check if first number is greater than second and third
    *   Print first is the greatest
*   Step 2: Check if second number is greater than first and third
    *   Print second is the greatest
*   Step 3: Third number has to be greatest
    *   Print third is the greatest

## INPUT
```cpp
#include <iostream>
using namespace std;
int main ()
{
    int first, second, third;
    first=10,second=20,third=30;
    
    //comparing first with other numbers
    if ((first >= second) && (first >= third))
        cout << first << " is the greatest "; 

    //comparing Second with other numbers 
    else if ((second >= first) && (second >= third))
        cout << second << " is the greatest";
    
    else
        cout << third << " is the greatest";
 
    return 0;
}
// Time complexity : O(1)
// Space complexity : O(1)
```
## OUTPUT
```
30 is the greatest
```

# Method 2:

### Working

For user inputs of numbers as first, second and third.

This method requires you know how ternary operator in C++ works

*   Step 1: Store the largest between first and second using ternary operator in variable temp
    *   temp = first > second ? first:second;
*   Step 2: Store the largest between temp and third using ternary operator in variable result
    *   result = temp > third ? temp:third;
*   Step 3: Print value of result

## INPUT
```cpp
#include <iostream>
using namespace std;
int main ()
{
    int first, second, third;
    
    first=10,second=20,third=30;
    
    int temp, result;

    // find the largest bw first and second and store in temp
    temp = first > second ? first:second;
    
    // find the largest bw temp and third and finally printing it
    result = temp > third ? temp:third;
        
    // the above two ternary statements can be condensed into one ternary statement
    //result = third > (first > second ? first : second) ? third : ((first > second) ? first : second);
    
    cout << result << " is the largest";

 
    return 0;
}
// Time complexity : O(1)
// Space complexity : O(1)
```
## OUTPUT
```
30 is the largest
```

# Method 3:

### Working

For user inputs of numbers as first, second and third.

This method uses internal inbuilt function max(a, b) which returns the larger value.

## INPUT
```cpp
#include <iostream>
#include <algorithm>
using namespace std;

int main ()
{
    int first, second, third;
    
    first=10,second=20,third=30;
    
    int result;

    result =  max(first,max(second, third));
    
    cout << result << " is the largest";

 
    return 0;
}

// Time complexity : O(1)
// Space complexity : O(1
```
## OUTPUT
```
30 is the largest
```
