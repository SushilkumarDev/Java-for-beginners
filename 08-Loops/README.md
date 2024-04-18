# Loops - For, While, Do While

A loop is used to run same code again and again.

### For Loop

For loop is used to loop code specified number of times.

```java
for (int i = 0; i < 10; i++) {
    System.out.print(i);
}
//Output - 0123456789

```
Syntax - For loop statement has 3 parts
- Initialization => int i=0. Initialization happens the first time a for loop is run.
- Condition => i<10. Condition is checked every time before the loop is executed.
- Operation (Increment or Decrement usually) => i++. Operation is invoked at the start of every loop (except for first time).

For Loop Puzzles
- Any of 3 parts in a for loop can be empty.
- There can be multiple statements in Initialization or Operation separated by commas


#### Exercises

```java
MyNumber number = new MyNumber(9);

number.isPrime(); //Is a number Prime? 
//Hint : 5 => true, 7 => true, 11 => true, 6 => false

int sum = number.sumUptoN();//Sum of numbers upto n?
//1 + 2 + 3 + 4 + 5 + 6

int sumOfDivisors = number.sumOfDivisors();

number.printANumberTriangle();
//1
//1 2
//1 2 3
//1 2 3 4 
//1 2 3 4 5
```


### While Loop

```
int count = 0;

while(count < 5){//while this condn is true, loop is executed.
    System.out.print(count);
    count++;
}
//Output - 01234
```

```java
count = 5;
while(count < 5){//condn is false. So, code in while is not executed.
    System.out.print(count);
    count++;
}//Nothing is printed to output
```

> Do not forget the increment!

#### Exercises

```java

WhileNumberPlayer player = new WhileNumberPlayer(30);//limit

player.printSquaresUptoLimit();
//For limit = 30, output would be 1 4 9 16 25

player.printCubesUptoLimit();
//For limit = 30, output would be 1 8 27

```

### Do While Loop
- The difference between a while and a do while is that the code in do while is executed at least once. 
- In a do while loop, condition check occurs after the code in loop is executed once.

Do While loop Example 1
```java
int count = 0;
do{
    System.out.print(count);
    count++;
}while(count < 5);//while this condn is true, loop is executed.
//output is 01234
```

Do While loop Example 2
```java
count = 5;
do{
    System.out.print(count);
    count++;
}while(count < 5);
//output is 5
```


#### Exercise
- Ask user for a number. 
- Print the cube of the number. 
- Do this repeatedly until user enters a negative number.

```
Enter a number: 5
Cube is 125
Enter a number: 3
Cube is 27
Enter a number: -1
Thank You! Have Fun!
```
### Break Statement

Break statement breaks out of a loop

Example 1
```java
for (int i = 0; i < 10; i++) {
    System.out.print(i);
    if (i == 5) {
         break;
    }
}

//Output - 012345
//Even though the for loop runs from 0 to 10, execution stops at i==5 because of the break statement. ÒBreak statementÓ stops the execution of the loop and takes execution to the first statement after the loop.
```

Break can be used in a while also.
```java
int i = 0;
while (i < 10) {
    System.out.print(i);
    if (i == 5) {
break;
    }
    i++;
}
//Output - 012345
```
Break statement takes execution out of inner most loop.
```java
for (int j = 0; j < 2; j++) {
    for (int k = 0; k < 10; k++) {
System.out.print(j + "" + k);
if (k == 5) {
    break;//Takes out of loop using k
}
    }
}
//Output - 000102030405101112131415
//Each time the value of k is 5 the break statement is executed. 
//The break statement takes execution out of the k loop and proceeds to the next value of j.

```
### Continue Statement
- Continue statement skips rest of the statements in the loop and starts next iteration

```java
for (int i = 0; i < 10; i++) {
    if (i == 5) {
      continue;
    }
    System.out.print(i);
}

//Output => 012346789

//Note that the output does not contain 5. 
//When i==5 continue is executed. Continue skips rest of the code and goes to next loop iteration. 
//So, the print statement is not executed when i==5.

```