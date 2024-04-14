# Conditionals

## Problem : Designing a Menu

- Ask User for input
  - Enter two numbers 
  - Choose an Operation
      - add
      - multiply
      - divide 
      - subtract
      - ...
  - Publish Result

```
Enter Number1: 
2

Enter Number2: 
4

1 - Add
2 - Subtract
3 - Divide
4 - Multiply
Choose Operation: 4

Result is - 8
```

```

```
## Basics of If Statement

- Conditionally execute code! 

> Code inside If is executed only if the condition is true.

// Basic Example
```
if(true){
    System.out.println("Will be printed");
}

if(false){
    System.out.println("Will NOT be printed");//Not executed
}

//Example 1
int x = 5;

if(x==5){
    System.out.println("x is 5");//executed since x==5 is true
}

//Example 2
x = 6;
if(x==5){
    System.out.println("x is 5");//Not executed since x==5 is false
}
//Example 3
int y = 10;

if(y==10){
    System.out.println("Y is 10");//executed-condn y==10 is true
} else {
    System.out.println("Y is Not 10");
}

//Example 4
y = 11;

if(y==10){
    System.out.println("Y is 10");//NOT executed
} else {
    System.out.println("Y is Not 10");//executed
}
//Example 5
int z = 15;
//Only one condition is executed. Rest of the conditions are skipped.
if(z==10){
    System.out.println("Z is 10");//NOT executed
} else if(z==12){
    System.out.println("Z is 12");//NOT executed
} else if(z==15){
    System.out.println("Z is 15");//executed. 
} else {
    System.out.println("Z is Something Else.");//NOT executed
}

z = 18;
if(z==10){
    System.out.println("Z is 10");//NOT executed
} else if(z==12){
    System.out.println("Z is 12");//NOT executed
} else if(z==15){
    System.out.println("Z is 15");//NOT executed
} else {
    System.out.println("Z is Something Else.");//executed
}
//If else Example: without Blocks
int number = 5;
if(number < 0) 
    number = number + 10; //Not executed
    number++; //This statement is not part of if. Executed.
System.out.println(number);//prints 6
```
## If else Puzzles

```
//Puzzle 1
int k = 15;
if (k > 20) {
    System.out.println(1);
} else if (k > 10) {
    System.out.println(2);
} else if (k < 20) {
    System.out.println(3);
} else {
    System.out.println(4);
}
```
//Output is 2. 
//Once a condition in nested-if-else is true the rest of the code is not executed.  
```
//Puzzle 2
int l = 15;

if(l<20)
    System.out.println("l<20");
if(l>20)
    System.out.println("l>20");
else
    System.out.println("Who am I?");
//Output is "l<20" followed by "Who am I?" on next line. 
//else belong to the last if before it unless brackets ({}) are used.
```
Puzzle 3

```
int m = 15;

if(m>20)
    if(m<20)
System.out.println("m>20");
    else
System.out.println("Who am I?");

//Nothing is printed to output. 

//Code above is similar to the code snippet shown below

if(m>20) {//Condn is false. So, code in if is not executed
    if(m<20)
System.out.println("m>20");
    else
System.out.println("Who am I?");
}
```
Puzzles Continued

```

//Puzzle 4

int x1 = 0;
//Condition in if should always be boolean
//if(x1) {} //COMPILER ERROR
//if(x1=0) {}//COMPILER ERROR. Using = instead of ==
//If else condition should be boolean
```

```
//Puzzle 5

boolean isTrue = false;

if(isTrue==true){
    System.out.println("TRUE TRUE");//Will not be printed
}

if(isTrue=true){
    System.out.println("TRUE");//Will be printed.
}

//Condition is isTrue=true. This is assignment. Returns true. So, code in if is executed.
```

Puzzle - Variables in a block


## Implementing Menu with if else

```
package com.in28minutes.primitive.datatypes;

import java.util.Scanner;

public class BasicMenu {
  public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);
    
    System.out.println("Enter Number1: ");
    int number1 = scanner.nextInt();
    
    System.out.println("Enter Number2: ");
    int number2 = scanner.nextInt();
    
    System.out.println("Add: 1");
    System.out.println("Subtract: 2");
    System.out.println("Choose Operation: ");
    int choice = scanner.nextInt();
    
    int result = 0;
    if(choice==1) {
      result = number1 + number2;
    } else if(choice == 2) {
      result = number1 - number2;
    }
    
    System.out.println(result);
  }

}

```