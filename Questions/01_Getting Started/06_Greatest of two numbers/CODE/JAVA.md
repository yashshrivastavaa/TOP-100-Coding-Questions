# Method 1 : Using if-else Statements

In this method we’ll use if-else statements to compare the two numbers and two numbers and print out the greatest.

### Algorithm

For the two given user inputs number1 and number2

* Check if both the integers are equal, print “Equal” if true.
* Check if number1>number2, print number1 if true.
* Check if number2>number1, print number2 if true.

Let’s implement the working in Java Language.

## INPUT
```Java
// Write a program to find the largest of two numbers in java
public class Main
 {
   public static void main (String[]args)
   {

     int num1 = 50, num2 = 20;
     if (num1 == num2)
       System.out.println ("both are equal");
     else if (num1 > num2)
         System.out.println (num1 + " is greater");

     else
         System.out.println (num2 + " is greater");

   }
 }
```
## OUTPUT
```
50 is greater
```

# Method 2 : Using Ternary Operator

In this method we’ll use the Ternary Operator and compare the two numbers to check for the greatest among them.

> Ternary Operator Syntax: 
> ( Condition ) ? ( if True : Action ) : ( if False : Action )

### Algorithm

For the given integer inputs number1 and number2

* Initialize the required variable.
* Check for the greatest among the two using Ternary Operator.

Let’s implement the working in Java Language.

## INPUT
```Java
public class Main
{
  public static void main (String[]args)
  {
    int num1 = 50, num2 = 10, temp;

    if (num1 == num2)
      System.out.println ("Both are Equal\n");
    else
      {
	temp = num1 > num2 ? num1 : num2;
	System.out.println (temp + " is largest");
      }

  }
}
```
## OUTPUT
```
50 is largest
```

# Method 3 : Using inbuilt max Function

In this method we’ll use the inbuilt max function to get the greatest of the two integer inputs.

### Algorithm

For the two integer inputs number1 and number2

* Initialize the required variables.
* Call the inbuilt max function with number1 and number2 as arguments.
* Print the returned value.

Let’s implement the working in Java Language.

## INPUT
```Java
public class Main {
    public static void main(String args[])
    {
        int num1 = 12, num2 = 21;
        if (num1 == num2)
            System.out.println("both are equal");
        else
            // prints the maximum of two numbers
            System.out.println(Math.max(num1, num2) + " is greater");
    }
}
```
## OUTPUT
```
21 is greater
```