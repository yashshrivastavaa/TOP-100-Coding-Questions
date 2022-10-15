# Method 1 : Using if-else Statements 1

## INPUT
```Java
// Write a program to find the largest of two numbers in java
public class Main
{
  public static void main (String[]args)
  {

    int num1 = 10, num2 = 20, num3 = 30;

    //checking if num1 is greatest
    if (num1 >= num2 && num1 >= num3)
        System.out.println (num1 + " is the greatest");

    //checking if num2 is greatest
    else if (num2 >= num1 && num2 >= num3)
        System.out.println (num2 + " is the greatest");

    //checking if num2 is greatest
    else if (num3 >= num1 && num3 >= num2)
        System.out.println (num3 + " is the greatest");
  }
}
```
## OUTPUT
```
30 is the greatest
```

# Method 2 : Using if-else Statements 2

## INPUT
```Java
public class Main
{
  public static void main (String[]args)
  {

    int num1 = 10, num2 = 20, num3 = 30;

    //comparing num1 with other numbers
    if ((num1 >= num2) && (num1 >= num3))
        System.out.println (num1 + " is the greatest");

    //checking if num2 is greatest
    else if (num2 >= num1 && num2 >= num3)
        System.out.println (num2 + " is the greatest");

    // num3 has to be greatest then if not above
    else
        System.out.println (num3 + " is the greatest");
  }
}
```
## OUTPUT
```
30 is the greatest
```

# Method 3 : Using inbuilt max Function

In this method we use the knowledge of Ternary Operators in Java.

> Ternary Operator Syntax: 
> ( Condition ) ? ( if True : Action ) : ( if False : Action )

## INPUT
```Java
public class Main
{
  public static void main (String[]args)
  {

    int num1 = 10, num2 = 20, num3 = 30;

     int temp, result;    
    
    // find the largest b/w num1 and num2 & store in temp
    temp = num1>num2 ? num1:num2;
    
    // find the largest b/w temp and num3 & finally printing it
    result = temp>num3 ? temp:num3;  
    System.out.println (result + " is the greatest");
  }
}
```
## OUTPUT
```
30 is the greatest
```