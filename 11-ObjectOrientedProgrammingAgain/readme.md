# OOPS Again

### Objects have state and behaviour

Fan Class
- State (Member Variables)
  - make;
  - radius;
  - color;
  - isOn;
  - speed;
- Constructors
  - Fan(String make, double radius, String color) 
- Behavior (Member Methods)
  - void switchOn()
  - void switchOff()
  - void changeSpeed()
  - String toString() using String.format method

  Exercise

- public class Rectangle
  - length, width;
  - What constructors?
  - What Operations?

### Object Composition

Customer
- homeAddress
- workAddress

#### Exercise
Book > id, name, author
 > Reviews > id, description, rating

```java 
 Book book = 
    new Book(123, "Object Oriented Programming with Java", 
          "Ranga");
 book.addReview(
    new Review(10, "Great Book", 5));
 book.addReview(
    new Review(101, "Awesome", 5);

 System.out.println(book);
 ```
## Inheritance Basics

### Inheritance Basics

public class Person name,phone,email;

- Student 
  - college
  - class
- Employee 
  - title
  - employer
  - employeeGrade
  - salary
  - toString (print all values including those of Person)

### Apply Inheritance to Savings Account

### More about Inheritance
- Method Overriding
- Is a relationship is mandatory
- Example in Java Api : HashMap & TreeMap extend AbstractMap.

## Inheritance Puzzles

Every Class extends Object class

Super class reference variable can hold an object of sub class

```
//Object is super class of all java classes
Object object = new Hero(); 
```
Multiple Inheritance results in a number of complexities. Java does not support Multiple Inheritance.

```
class Dog extends Animal, Pet { //COMPILER ERROR
}
```

We can create an inheritance chain.
```
class Pet extends Animal {
}

class Dog extends Pet {
}
```
instanceof operator checks if an object is of a particular type.

- Can be used with Interfaces and Classes


### Inheritance and Constructors
 - A constructor can call the constructor of a super class using the super() method call. Only constraint is that it should be the first statement.
 - Another constructor in the same class can be invoked from a constructor, using this({parameters}) method call.
 - If a super class constructor is not explicitly called from a sub class constructor, super class (no argument) constructor is automatically invoked (as first line) from a sub class constructor.

Constructors are NOT inherited.
```
class Animal {
    String name;

    public Animal(String name) {
this.name = name;
System.out.println("Animal Constructor with name");
    }
}

class Dog extends Animal {
}

public class ConstructorExamples {
    public static void main(String[] args) {
// Dog dog = new Dog("Terry");//COMPILER ERROR
    }
}
```
## Abstract Class

### Basics of an Abstract Class

- An abstract class is a class that cannot be instantiated, but must be inherited from. An abstract class may be fully implemented, but is more usually partially implemented or not implemented at all, thereby encapsulating common methodality for inherited classes.
An abstract class cannot be instantiated.

### One more example of an Abstract Class

Cooking Recipe
- firstStep - Review Availability of Oven, Stove and Utensils
- The usual recipe steps
- lastSteps - Switch off microwave oven, stove and clean everything!

### Abstract Class Puzzles
Abstract class can contain instance and static variables
//An Abstract method does not contain body.
//Abstract Class can contain ZERO or more abstract methods
//Abstract method does not have a body
//Abstract class can contain fully defined non-abstract methods. 

// A concrete sub class should implement all abstract methods.
// Below class gives compilation error if uncommented

## Interface Basics

A lot of confusion between Interface and Abstract Class. They are very different. We need to get our thinking right about interfaces. Interfaces have nothing to do with Inheritance.

What does the word interface represent to you? Think about it.

What is the interface that a Video game console provides you with?

Interface of a Video game console exposes what actions you can perform with it.
 - It exposes the interfaces for the buttons
      - Left, right, up, down, green, red, blue

What would the game writer do? Provide implementations for those methods. 

Thats the best way to think about interfaces! What are the actions that can be performed? Represent that as an interface. 

### First example with an interface

VideoGameConsole
> MarioGame
> PacmanGame
> ChessGame
