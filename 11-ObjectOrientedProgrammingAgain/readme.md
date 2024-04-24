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