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
