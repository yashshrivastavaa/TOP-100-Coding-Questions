# Method 1: Using Brute Force

This method uses Brute Force to check whether a given integer is Positive or Negative.

## INPUT
```Python
num = 15
if num > 0:
    print('Positive')
elif num < 0:
    print('Negative')
else:
    print('Zero')
```
## OUTPUT
```
Positive
```

### Algorithm

This method uses Brute Force to check whether a given integer is Positive or Negative.

Algorithm for the above code is as follows,

*   Initialize num as 15
*   If the num > 0: it is a positive number.
*   If the num < 0: it is a positive number.
*   Else the number has to be zero itself

# Method 2: Using Nested if-else Statements

This method uses a nested if-else Statements to check whether a given number is Positive or Negative.

## INPUT
```Python
num = 15
if num>=0:
    if num==0:
        print('Zero')
    else:
        print("Positive")
else:
    print("Negative")
```
## OUTPUT
```
Positive
```

### Algorithm

This method uses a nested if-else Statements to check whether a given number is Positive or Negative.

Algorithm for the above code is as follows,

*   Initialize num as 15
*   If the num >= 0
    *   If num == 0 : num is zero
    *   Else number has to be positive 
*   Else the number has to be negative

# Method 3: Using Ternary Operator

This method uses a ternary operator to check whether a number is Positive or Negative.

> Ternary Operator Syntax: 
> ( Condition ) ? ( if True : Action) : ( if False : Action) ;

## INPUT
```Python
num = 15
print("Positive" if num>=0 else "Negative")
```
## OUTPUT
```
Positive
```

### Algorithm

This method uses a ternary operator in Python to check whether a number is Positive or Negative.

For a user input num

*   Return “Positive” if num>=0 else “Negative”.

Algorithm for the above code is as follows,

*   Initialize num as 15.
*   print the output using ternary operator in python using print () function.