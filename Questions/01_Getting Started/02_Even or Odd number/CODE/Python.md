# Method 1: Using Brute Force

This method simply checks if the given input integer is divisible by 2 or not. If it’s divisible then print Even or Odd otherwise.

## INPUT
```Python
num = int(input("Enter a Number:")) 
if num % 2 == 0: 
  print("Given number is Even") 
else: 
  print("Given number is Odd")
```
## OUTPUT
```
Enter a Number: 5 
Given number is Odd
```

### Algorithm

The working of the above mentioned code is as follows,

*   Start
*   Insert a number.
*   If the given number is divisible by 2, then print,” Given number is even”.
*   If the given number is not divisible by 2, then print ,”Given number is odd”.
*   Stop

### Explanation

Given an integer as input, the objective is check whether the number is even or odd in Python. To do so we check if it’s divisible by 2 or not. If true, it’s even or it’s odd otherwise.

The algorithm for the above code is as given below,

*   Import the required modules using import keyword.
*   Initialize the required variables.
*   Check if the number is divisible by 2, if true print even or odd otherwise using print() function.

The output for the above code is wither even or odd based on whether or not it’s divisible by 2.

# Method 2: Using Ternary Operator

This Method uses the ternary operator to check if the integer input is divisible by 2, If true print Even or Odd otherwise.

> Ternary Operator Syntax Python: 
> ( True : Action ) if ( Condition ) else ( False : Action )

## INPUT
```Python
num = 17
print("Even") if num%2 == 0 else print("Odd")
```
## OUTPUT
```
Odd
```

### Algorithm

The working of the above code is as follows,

*   Input an integer input num.
*   Check whether the number is divisible by 2 using the ternary operator
*   Ternary Operation, print(“Even”) if (num%2 == 0) else (print(“Odd”))

### Explanation

Given an integer as input, the objective is check whether the number is even or odd in Python. To do so we check if it’s divisible by 2 or not using a Ternary Operator in Python. If true, it’s even or it’s odd otherwise.

The algorithm for the above code is as given below,

*   import the required modules using import keyword.
*   Initialize the required variables.
*   Check if the number is divisible by 2 using a Ternary Operator, if true print even or odd otherwise using print() function.

The output for the above code is wither even or odd based on whether or not it’s divisible by 2.

# Method 3: Using Bitwise Operator

This Method uses bitwise operators to check if a given number is Even or Odd.

> Bitwise Operators: 
> In computer programming, a bitwise operation operates on a bit string, a bit array or a binary numeral at the level of its individual bits. It is a fast and simple action, basic to the higher-level arithmetic operations and directly supported by the processor.

## INPUT
```Python
def isEven(num):
  return not num&1

if __name__ == "__main__":
  num = 13
  if isEven(num):
    print('Even')
  else:
    print('Odd')
```
## OUTPUT
```
Odd
```

### Algorithm

The working of the above code is as follows,

*   If we have any number num doing bitwise ‘&‘ operation will give resultant as
    *   1: If n is odd
    *   0: if n is even

### Explanation

Given an integer as input, the objective is check whether the number is even or odd in Python. To do so we check if it’s divisible by 2 or not using Bitwise Operator. If true, it’s even or it’s odd otherwise.

The algorithm for the above code is as given below,

*   Import the required modules using import keyword.
*   Define a function isEven() which returns a boolean variable to check if the number is even or odd.
*   Initialize the required variables.
*   Check if the function after calling returns True or False, if true print even or odd otherwise using print() function.

The output for the above code is wither even or odd based on whether or not it’s divisible by 2.