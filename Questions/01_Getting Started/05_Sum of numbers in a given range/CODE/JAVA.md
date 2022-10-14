# Method 1 : Using for Loop

In this method we’ll use for loop to iterate through the numbers in a range of [0,num].

### Algorithm

For an integer input “num” we do the following

* initialize the required variables within the class.
* Run a for loop from 0 to num+1 meanwhile appending all the numbers to sum variable.
* Print the sum variable.

Let’s implement the logic in Java Language.

## INPUT
```Java
public class Main
 {
   public static void main (String[]args)
   {

     int n = 10;
     int sum = 0;

     for (int i = 1; i <= n; i++)
         sum += i;
       System.out.println (sum);
   }
 }
```
## OUTPUT
```
55
```

# Method 2 : Using the Formula

In this method we’ll use a formula to find the sum of N integers in a series from sequence and series. The formula is mentioned below.

> Formula to Find the Sum of N Integers: 
> Sum = num * ( num + 1 ) / 2

### Algorithm

For an integer input we do the following operations

* Initialize the following variables.
* Implement the formula as sum = num * ( num + 1 ) / 2.
* Print the sum variable.

Let’s implement the above logic in Java language.

## INPUT
```Java
public class Main
 {
   public static void main (String[]args)
   {

     int n = 10;

       System.out.println ( n*(n+1)/2);
   }
```
## OUTPUT
```
55
```

# Method 3 : Using Recursion

In this method we’ll use the concept of recursion to find the sum of all the number that lay from 0 to num. To know more about recursion, check out Recursion in Java

### Algorithm

For a given integer input as “num” we perform the following steps

* Initialize the required variables.
* Define a recursive function with base case as num == 0.
* Set recursive step call as num + recursum(num-1).
* Call the recursive function and print the value returned by the function.

Let’s implement the above logic in Java Language.

## INPUT
```Java
public class Main
{
  public static void main (String[]args)
  {

    int n = 10;
    int sum = getSum (n);

      System.out.println (sum);
  }

  static int getSum (int n)
  {
    if (n == 0)
      return n;

    return n + getSum (n - 1);
  }
}
```
## OUTPUT
```
55
```