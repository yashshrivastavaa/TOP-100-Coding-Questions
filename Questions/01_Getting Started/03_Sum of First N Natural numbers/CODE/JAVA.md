# Method 1 : Using Brute Force

This method simply checks if the given input integer is divisible by 2 or not. If it’s divisible then print Even or Odd otherwise.


### Algorithm

The working of the above code is mentioned below

* Input an integer input “number“
* Check whether the number is divisible by 2
* This means using modulo/remainder operator leaves 0 as a remainder
* Do : if (number % 2 == 0)
  * if yes, print “Even number”
  * if not, print “Odd number”

## INPUT
```Java
public class Main
 {
      public static void main(String[] args) {
           int number = 29;


     //checking whether the number is even or odd
     if (number % 2 == 0)
              System.out.println(number + " is Even");
     else
              System.out.println(number + " is odd");
      }
 }
```
## OUTPUT
```
29 is Odd 
```

# Method 2: Using Ternary Operator

This Method uses the ternary operator to check if the integer input is divisible by 2, If true print Even or Odd otherwise.


### Algorithm

The working of the above code is as follows,

* Input an integer input “number“
* Check whether the number is divisible by 2 using the ternary operator
* (number % 2) ? (cout <<“Even”) : (cout << “Odd”)

## INPUT
```Java
public class Main
 {
   public static void main (String[]args)
   {
     int number = 29;

     //Checking if the number is divisible by 2
     String status = number % 2 == 0 ? " is Even" : " is Odd";
       System.out.println (number + status);
   }
 }
```
## OUTPUT
```
 29 is Odd
```

# Method 3: Using Bitwise Operator

This Method uses bitwise operators to check if a given number is Even or Odd.

> Bitwise Operators: 
> In computer programming, a bitwise operation operates on a bit string, a bit array or a binary numeral at the level of its individual bits. It is a fast and simple action, basic to the higher-level arithmetic operations and directly supported by the processor


### Algorithm

The working of the above code is as follows,

* If we have any number ‘n‘ doing bitwise ‘&‘ operation will give resultant as
  * 1: If n is odd
  * 0: if n is even

## INPUT
```Java
public class Main
{
  public static void main (String[]args)
  {
    int number = 29;

    if (isEven (number))
        System.out.println ("Even");
    else
        System.out.println ("Odd");
  }


// Returns true if n is even, else odd
  static bool isEven (int number)
  {

    // n & 1 is 1, then odd, else even
    return (!(number & 1));
  }
}
```
## OUTPUT
```
Odd
```