# Method 1 : Using for Loop

In this method we’ll add all the natural numbers until the given integer input using for loop in Python.

## INPUT
```Python
num = 5
sum = 0
for i in range(num+1):
  sum+=i
print(sum)
```
## OUTPUT
```
15
```

### Working

For a user input num.

* Initialize a variable sum = 0.
* Using a for loop in iteration ‘i’ iterate between [1, num].
* Each time add ‘i’ to current sum as sum = sum + i.
* Print sum.

### Explanation

Given an integer input N, the objective is to calculate the sum of all the natural numbers until the integer N. To do so we iterate through all the numbers that lay within N and keep incrementing the sum value.

The algorithm for the above code is as follows,

* Import the required module using the import keyword.
* Initialize the required variables.
* Run a for loop with range as N+1.
* Keep adding the iter values to the Sum variable.
* Print Sum variable using print() function.

The output for the above mentioned code is the sum of all the natural numbers until the given value.

# Method 2: Using Formula for the Sum of Nth Term

In this Method we use the formula for finding the sum of N term.

> Formula to Find the Sum of N terms: 
> Sum = ( Num * ( Num + 1 ) ) / 2

## INPUT
```Python
num = 5
print(int(num*(num+1)/2))
```
## OUTPUT
```
15
```

### Working

For a user input n.

* Initialize a variable sum = 0.
* Use formula sum = n(n+1)/2.
* Print sum

### Explanation

Given an integer input N, the objective is to calculate the sum of all the natural numbers until the integer N. To do so we iterate through all the numbers that lay within N and keep incrementing the sum value.

The algorithm for the above code is as follows,

* Import the required modules using the import keyword.
* Initialize the required variables.
* Run a for loop with range as N+1.
* Keep adding the iter values to the Sum variable.
* Print Sum variable using print() function.

This algorithm uses the formula n(n+1)/2 that can be used to find sum of first N natural numbers. This also reduces the time complexity from O(n) to O(1). The output for the above mentioned code is the sum of all the natural numbers until the given value.

# Method 3: Using Recursion

This method uses Recursion to recursively add the natural numbers up to the given integer input using recursion in c++.

## INPUT
```Python
def getSum(num):
  if num == 1:
    return 1
  return num + getSum(num-1)

num = 5
print(getSum(num))
```
## OUTPUT
```
15
```

### Working

For a user input n.

* Initialize a variable sum = 0.
* Call function getSum (num).
* In each recursive call add the current value of n and call for lower recursion call using return num + getSum(num-1);
* Print sum value

### Explanation

Given an integer input N, the objective is to calculate the sum of all the natural numbers until the integer N. To do so we recursively call a function  iterate through all the numbers that lay within N and keep incrementing the sum value.

The algorithm for the above code is as follows,

* Import the required modules using the import keyword.
* Define a Recursive function getSum() which takes the number input as an argument.
* Recursively call the function and keep on adding the return statements.
* Initialize the required variables.
* Call the Recursive function and print out the returned value using cout keyword.

The output for the above mentioned code is the sum of all the natural numbers until the given value.