# Method 1 : Using if-else Statements 1

In this method we’ll use the if-else statements to check whether or not the input integer satisfies either of the conditions. To learn more about control statements in python, check out if-else control statements in Python.

### Working

For a User Input year we do

* Check if the year variable is divisible by 400.
* Check if the year variable is divisible only by 4 and not 100.
* If the above mentioned conditions are satisfied, prints “Leap Year”, print “Not a Leap Year” otherwise.

Let’s implement the above logic in Python Language.

## INPUT
```Python
year = 2000
if (year%400 == 0) or (year%4==0 and year%100!=0):
  print("Leap Year")
else:
  print("Not a Leap Year")
```
## OUTPUT
```
Leap Year
```

# Method 2: Using if-else Statements 2

In this method we’ll use the if-else statements to check whether or not the input integer satisfies either of the conditions. This method is a modified and simpler version of the previous method.

### Working

For a User Input year we do

* The input is stored in an int type variable say year.
* year is checked for being a leap year or not with the following condition if( ((year % 4 == 0)&&(year % 100 != 0)) || (year % 400==0) )
* If the above condition is true then input is a leap year otherwise input is not a leap year.

Let’s implement the above logic in Python Language.

## INPUT
```Python
year = 2000
if( ((year % 4 == 0) and (year % 100 != 0)) or (year % 400==0) ):
    print("Leap Year")
else:
    print("Not leap Year")
```
## OUTPUT
```
Leap Year
```