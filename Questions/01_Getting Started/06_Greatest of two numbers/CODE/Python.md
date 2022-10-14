# Method 1 : Using Brute Force

In this method we’ll use loops like for, while and do while to sum all the numbers that lay in the intervals of the given input integers.

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

### Working

For in integer inputs num1 and num2 as the intervals

* Initialize the required variables.
* Run a for loop from num1 to num2+1 i.e [num1,num2].
* Append i to sum variable with each iteration.
* Print sum variable.

Let’s implement the above logic in Python Language.

# Method 2: Using the Formula

In this method we’ll use formula mentioned below to find the sum of all the numbers that lay in the interval given by the input variable.

> Formula to Find the Sum of Numbers in an Interval: 
> The formula to find the sum of n natural numbers is:
> Sum = n * ( n + 1 ) / 2
> 
> Therefore in order to find the sum in a given interval we'll minus the sum of the numbers until the lower range from the whole sum and add an offset as the lowest bound is itself included in the summation. Hence the final formula is :
> Sum = b * ( b + 1 ) / 2 – a * ( a + 1 ) / 2 + a .

## INPUT
```Python
num1, num2 = 3, 6
sum = int((num2*(num2+1)/2) - (num1*(num1+1)/2) + num1)
print(sum)
```
## OUTPUT
```
18
```

### Working

For the two integer inputs num1 and num2

* Initialize the required variables.
* perform sum = int((num2*(num2+1)/2) – (num1*(num1+1)/2) + num1).
* Print Sum variable.

Let’s implement the above logic in Python Language.

# Method 3: Using Recursion

In this method we’ll use recursion to find the sum of all the numbers that lay in the interval given by the input variable. To know more about recursion, refer to Recursion in Python.

## INPUT
```Python
def recursum(sum,num1,num2):
  if num1 > num2:
    return sum
  return num1 + recursum(sum,num1+1,num2)

num1, num2 = 3, 6
sum = 0
print(recursum(sum,num1,num2))
```
## OUTPUT
```
18
```

### Working

For the two integer inputs num1 and num2 as the interval

* Initialize the required variables.
* Define a recursive function with base case as num1>num2.
* Set the recursive step call as num1 + recursum(sum, num1+1, num2).
* call the recursum() function and print the returned value.

Let’s implement the above logic in Python Language.