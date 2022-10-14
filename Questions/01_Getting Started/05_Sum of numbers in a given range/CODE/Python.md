# Method 1 : Using for Loop

In this method we’ll add all the natural numbers until the given integer input using for loop in Python.

## INPUT
```Python
number,sum = 6,0
for i in range(number+1):
  sum+=i
print(sum)
```
## OUTPUT
```
21
```

### Working

For an integer input “number” we do the following

* Initialize the required variables.
* Using for loop iterate from 0 to number+1.
* Meanwhile append the number to sum variable.
* Print the sum variable.

Let’s implement the above logic in Python code.

# Method 2: Using the Formula

In this method we’ll use the formula for finding the sum of N integers in a series from series and sequences i.e sum = number * ( number + 1 ) / 2 to calculate the sum until the given integer input.

## INPUT
```Python
number = 6
sum = int((number * (number + 1))/2)
print(sum)
```
## OUTPUT
```
21
```

### Working

For an integer input “number”  we perform the following steps

* Initialize sum variable as sum = (number * ( number + 1 ) /2 ).
* Print the sum variable.

Let’s implement the above logic in Python Language.

# Method 3: Using Recursion

In this method we’ll use recursion to recursively iterate through the number while appending them to the sum variable until the number is reach which here act as the base case. To learn more about recursion, check out Recursion in Python.

## INPUT
```Python
ddef recursum(number):
  if number == 0:
    return number
  return number + recursum(number-1)
number, sum = 6,0
print(recursum(number))
```
## OUTPUT
```
21
```

### Working

For an integer input “number” we do

* Initialize the required variables.
* Define a recursive function with base case as number ==0.
* Set the step recursive call as number + recursum( number – 1 ).
* Call the recursive function recursum() and print the returned value.

Let’s implement the above logic using Python Language.