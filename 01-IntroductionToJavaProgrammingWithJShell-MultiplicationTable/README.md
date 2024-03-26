## I Love Programming
- Fun
- Solving Problems


## Learning Programming
- Problem Solving Skills
- Concepts
- Language Specifics

## JShell

- Java REPL Read Eval Print Loop
- Type in one line of code (or multiple) and see output
- Makes learning Fun
- Introduced in Java 9

## Concepts
- JShell
- Statements
- Expressions
- Variables
- Literals
- If Statement
- For Loop
- Method/Function

## Multiplication Table
```
5 * 1 = 5
5 * 2 = 10
5 * 3 = 15
5 * 4 = 20
5 * 5 = 25
5 * 6 = 30
5 * 7 = 35
5 * 8 = 40
5 * 9 = 45
5 * 10 = 50
```
## Multiplication Table - Step By Step
- How to break it down?
- Where do we start?
- Calculate 5 * 5
- Print 5 * 5 = 25
- Do this 10 Times

## Naming a Variable/Method
- Combination of letters, numbers, $ and under-score(_)
- Cannot start with a number
- Cannot be a keyword
- No limit on length of identifier
- CamelCase

## Variables Types
- byte  b = 5;             //8  bits - 128 to 127
- short   s = 128;         //16 bits - 32,768 to 32,767 
- int     i = 40000;      //32 bits -  2,147,483,648 to 2,147,483,647
- long  l = 222222222; //64 bits -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807
- float   f = 4.0f;          //32 bits NOT VERY PRECISE - don’t use for financials
- double  d = 67.0; //64 bits NOT VERY PRECISE - don’t use for financials
- char  c = 'A';             //16 bits '\u0000' to '\uffff'
- boolean isTrue = false;  //true or false


## Launch JShell

JShell
- [x] Java REPL Read Eval Print Loop
- [x] Type in one line of code (or multiple) and see output
- [x] Makes learning Fun
- [x] Introduced in Java 9

# What is Programming all about?

I Love Programming
- [x] Fun
- [x] Solving Problems

Why do you think I love programming? Because I think programming is a lot of fun. I love solving problems and I love having fun. And the combination is awesome.

In this course, we would want to help you to develop a love for programming. If you had bad experiences in learning programming earlier, forget about them. 
Start fresh and I promise - This will be an awesome roller coaster ride! 

Let's take a step back and think what are the important things that you would want to learn to be a great programmer

Learning Programming
- [x] Problem Solving Skills
- [x] Concepts
- [x] Language Specifics

As a programmer, you want to solve problems. You want to be able to get the computer to do things for you. To be able to do that you need problem solving skills. You would need to be able to look a problem and identify the approach to solve it - How to break the problem down? Which programming concepts to use? How to express them in the language you've chosen?

There are Three parts to learning programming
- Concepts - Programming Concepts like variables, methods, OOPS etc
- Syntax - Understanding programming constructs
- Solving Problems - Breaking them into sub problems and working towards a solution

While all this looks complex, we will make it easy for you by solving a variety of challenges. We will start with basic challenges like multiplication table and increase the difficulty level during the course.

Our focus in this course is on two things a)Have Fun b)Solve Problems.

First steps with programming are the most difficult ones. Its like learning to ride a bicycle. The learning curve is steep initially. Once you get hang of it, it becomes easier.

We would want to give you a holding hand during the initial stages of the course so that you make less mistakes and have help to fall back on if you have problems
- Attached is a 50(XXXXX) page pdf with this lecture. You can use that as a reference if you are unable to get something working.

## First Challenge

Our first challenge is to get the computer to print a multiplication table for us. Over the course of next few steps, we will work our way towards a simple multiplication program. 

```
for(int i=1;i<=10;i++) 
	System.out.printf("%d * %d = %d", 5 , i , 5 * i ).println();
```

```
5 * 1 = 5
5 * 2 = 10
5 * 3 = 15
5 * 4 = 20
5 * 5 = 25
5 * 6 = 30
5 * 7 = 35
5 * 8 = 40
5 * 9 = 45
5 * 10 = 50
```

At the end of these few steps, you will be able to write a simple program to do this and hopefully understand most parts of it!

Over the next few steps, you will learn 
- JShell
- statements
- expressions
- variables
- literals
- conditions
- if statement
- for loop
- methods or functions

## Launching JShell

Launch JShell

/exit to exit

Relaunch

## Multiplication Table - Step By Step
- [x] How to break it down?
- [x] Where do we start?
- [x] Calculate 5 * 5
- [x] Print 5 * 5 = 25
- [ ] Do this 10 Times

## First Java Expression

Next few videos, we assume that you are a beginner to programming. i.e. You wrote zero programs before! If you have a little bit of experience, you might find this a little slow but I'm sure with a little bit of patience you would love this. 


Let's get the computer to do a few calculations for us to get started.

> 10 + 5
15

> 10 * 5
50

> 10 - 5
5

> 10 - 5 * 2 //Think about this!

5

Terminology - operand, operator, literal
Numeric Operators -> + - / * /
What we are using are expressions to perform operations on numbers. +, *, - are operators.  The numbers are called Literals.

What we are using here is JShell.

A few puzzles
- 1 + 2 //Notice the spaces - Programming Languages do not worry about spaces - for the most part!
- 1+2//No spaces
- 5/2
- 5*2 + 2

Exercise
- Write an expression to calculate number of minutes in a day.
- Write an expression to calculate number of seconds in a day.

## More Operators and Precedence
- 1 + 5 * 2
- 5 % 2
- 5 / 2

Puzzles
- Basic Precedence of Operators * / > + - 
- Print a few complex expressions and see if you can work out how they work
- Use operator % 


## Printing output

Computer's cannot understand Human Languages. Computers have languages of their own - You are learn Java - which is one of the computer programming languages. For computers to understand you, we need to start understanding these programming languages. 

You can adjust the playspeed of the video if I'm speaking too fast. Look at the interface for the video player and you should find a speed icon!

How to write code to print something on the console or the output?

```
System.out.println("Welcome to Programming World");
```

Programming languages speak a different language - Rules are complex. These rules are called Syntax. Programming Languages don't like it when you don't follow the syntax. It's like your strict natural language instructor.

What can go wrong?
- JShell
- Case of the letters - Upper case and lower case
- Double Quotes
- Syntax of method - round brackets ()

Statement - An instruction to the computer. We instructed Java to print a text and it printed it.

Congratulations!

There are things we did not understand during our first statement. We will understand them now!

> Tip 1 - Using Arrows

### Method Call
System.out.println("Welcome to Programming World")
- This is a method call. We are calling a method. The syntax to call a method is method_name(value)
- In this example
	- method_name is System.out.println
	- value we want to print is "Welcome to Programming World"
- System.out.println is an inbuilt method provide by Java. It prints the value passed to it to the console i.e. the screen in JShell!

### Double Quotes
Any thing in double quote is considered as text. This is called a String Literal.

System.out.println(Welcome to Programming World)

System.out.println("Welcome to Programming World")

Puzzles
- Different Case - System.out.println("welcome to programming world")

Exercises
- Print "Hello World"
- Print "5 * 3"

## Text vs Expression

Let's make the computer do a few calculations for us.

System.out.println("5 * 6");//Doesn't work

System.out.println(5 * 6);//30 

Anything between quotes is taken as is. It is not computed. 

System.out.println(5 + 6);
System.out.println(5 - 6);
System.out.println(5 / 6); // Why is this Zero? Later

Awesome isn't it? We have the computer doing some work for us. That's what programmers are supposed to do. Get the computer to do something useful for us.

Do you know? 
- You have successfully executed more than 10 Java Statements in a very short span of time. That's because of the magic of a new Java 9 Feature - JShell.  Without JShell, getting started would've been more difficult

Tip
- Programming is all about understand what, why and how of what we do. It is not sufficient to say it works. You should be able to explain How it works? Why it works? To do this, start questioning everything. I mean E V E R Y T H I N G!


Exercise
- Try to print a simple math table executing individual statements
  	- System.out.println(5 * 1)
  	- System.out.println(5 * 2)
  	- System.out.println(5 * 3)


## More advanced System.out.println

I want to print 5 table in this format 
5 * 1 = 5

We have to write - System.out.println("5 * 1 = 5")

This is not fun. Computer is not calculating it for us! How to get it to calculate and print the value for us?

We will use a new function printf.

However printf has a few constraints
- System.out.printf("5 * 1 = 5") //No new line
- System.out.printf("5 * 1 = 5") //It returns a value
- System.out.printf("5 * 1 = 5").println() //Avoids all complication around it - This is called chaining of calls. Don't worry about it for now!

You can ask - why are we using printf? Because, it has an additional feature.

System.out.printf("5 * 1 = %d", 5 * 1).println();
System.out.printf("5 * 2 = %d", 5 * 2).println();

Now we got the computer do some calculations for us! That's cool.

Each of the values we send to printf are called parameters.

How about replacing the other things in the String (Any text within quotes is called a String) with a variable too?
System.out.printf("%d %d %d", 1 , 2 , 3 ).println();

System.out.printf("%d * %d = %d", 5 , 6 , 5 * 6 ).println();
System.out.printf("%d * %d = %d", 5 , 7 , 5 * 7 ).println();

Let's do a quick review
- In built method
- Literal
- Passing Parameters

Exercise
- Adding three numbers 5 + 6 + 7 = 18

