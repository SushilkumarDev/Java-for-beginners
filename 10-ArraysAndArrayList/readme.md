# Introduction to Array and ArrayList

## Challenge
```java
Student student = new Student (name, list of marks);
int number = student.getNumberOfMarks();
int sum = student.getTotalSumOfMarks();
int maximumMark = student.getMaximumMark();
int minimumMark = student.getMinimumMark();
BigDecimal average = student.getAverageMarks();
student.addNewMark(35);
student.removeMarkAtIndex(5);
```

## Concepts
 - Arrays
 - ArrayList

## Why do we need an Array?
- Arrays allow storing multiple values of same type.

## Array Basics

```
//Declaring an array

//Declaring and creating an array in same line.
int marks2[] = new int[5];

//You can Declare, Create and Initialize Array on same line.
int marks3[] = { 25, 30, 50, 10, 5 };

//Accessing values from an array

int length = marks.length;//Length of an array: Property length

//Index of elements in an array runs from 0 to length - 1
marks[0] = 25;
marks[1] = 30;
marks[2] = 50;
marks[3] = 10;
marks[4] = 5;

System.out.println(marks[2]);//Printing a value from array
```
Exercise 
- Print all values in an array
- Find sum of all values in an array
