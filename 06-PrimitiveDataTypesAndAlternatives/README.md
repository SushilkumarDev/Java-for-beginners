# Primitive Data Types in Depth

## Quick Revision

Primitive Data Types
- Integer
  - byte, short, int, long
- Floating Point 
  - float, double
- Boolean 
  - boolean
- Character
  - char

In-Depth
- Literals
- Operators
- Conversion (Casting)
- Use them in Classes

## Integer Data Types
- Default literal type is int. Long example - 40l or 40L
- There are 3 ways of representing an Integer Literal. 
  - Decimal. Examples: 343, 545
  - Octal. Digits 0 to 7. Place 0 before a number. Examples : 070,011
  - Hexadecimal. Digits 0 to 9 and alphabets A to F (10-15). Case insensitive.
- Operators are +, -, /, *, %, Increment and Decrement operators
- Implicit Conversion if literal fits in the variable type
- Explicit Conversion otherwise

```java
int eight = 010; 
int nine=011;  
int invalid = 089;//COMPILER ERROR! 8 and 9 are invalid in Octal
int sixteen = 0x10; 
int fifteen = 0XF; 
int fourteen = 0xe;
int x = 23,000;
long a = 123456789l; 
long b = 0x9ABCDEFGHL; 
long c = 0123456789L;

byte b = 10; //byte b = (int) 10; Example below compiles because compiler introduces an implicit cast.

short n1 = 5;
short n2 = 6;
//short sum = n1 + n2;//COMPILER ERROR
short sum = (short)(n1 + n2);//Needs an explicit cast

byte b = 5;
b += 5; //Compiles because of implicit conversion

int value = 100;
long number = value; //Implicit Casting

long number1 = 25678;
int number2 = (int)number1;//Explicit Casting
//int x = 35.35;//COMPILER ERROR
int x = (int)35.35;//Explicit Casting

int bigValue = 280;
byte small = (byte) bigValue;
System.out.println(small);//output 24. Only 8 bits remain.

//byte large = 128; //Literal value bigger than range of variable type causes compilation error
byte large = (byte) 128;//Causes Truncation!

int i = 25;
int j = ++i;//i is incremented to 26, assigned to j
System.out.println(i + " " + j);//26 26

i = 25;
j = i++;//i value(25) is assigned to j, then incremented to 26
System.out.println(i + " " + j);//26 25

```

Exercise
```java
   BiNumber numbers = new BiNumber(2, 3);
   System.out.println(numbers.add());
   System.out.println(numbers.multiply());
   numbers.double();//Double both numbers 
   System.out.println(numbers.getNumber1());
   System.out.println(numbers.getNumber2());
```