# Method 1 : Using Brute Force

In this method we’ll use loops like for, while and do while to sum all the numbers that lay in the intervals of the given input integers.

### Working

For the two integer inputs num1 and num2

* Check if num1>num2, print num1 if true.
* Print num2 otherwise.

Let’s implement the above logic in Python Language.

## INPUT
```Python
num1, num2 = 3, 6
sum = 0
for i in range(num1,num2+1):
  sum+=i
print(sum)
```
## OUTPUT
```
18
```

# Method 2: Using the Formula

In this method we’ll use formula mentioned below to find the sum of all the numbers that lay in the interval given by the input variable.

### Working

Given the integer inputs num1 and num2

* Check if num1>num2 using ternary operator in python.
* print num1 if true or num2 otherwise.

Let’s implement the above logic in Python Language.

## INPUT
```Python
num1, num2 = 20 , 30
print((num1 if num1>num2 else num2))
```
## OUTPUT
```
30
```

# Method 3: Using Recursion

In this method we’ll use recursion to find the sum of all the numbers that lay in the interval given by the input variable. To know more about recursion, refer to Recursion in Python.

### Working

Given two input numbers num1 and num2

* Call inbuilt max() function with num1 and num2 as arguments.
* Print the returned value.

Let’s implement the above logic in Python Language.

## INPUT
```Python
num1, num2 = 20, 30
print(max(num1,num2))
```
## OUTPUT
```
30
```

