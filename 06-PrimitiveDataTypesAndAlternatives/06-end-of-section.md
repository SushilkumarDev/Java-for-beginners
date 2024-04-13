<!---
Current Directory : /in28Minutes/git/java-a-course-for-beginners/6-PrimitiveDataTypesAndAlternatives
-->

## Complete Code Example


### /src/com/in28minutes/primitive/datatypes/BiNumber.java

```java
package com.in28minutes.primitive.datatypes;

public class BiNumber {
	private int number1;
	private int number2;

	public int getNumber1() {
		return number1;
	}

	public void setNumber1(int number1) {
		this.number1 = number1;
	}

	public int getNumber2() {
		return number2;
	}

	public void setNumber2(int number2) {
		this.number2 = number2;
	}

	public BiNumber(int number1, int number2) {
		this.number1 = number1;
		this.number2 = number2;
	}

	public int add() {
		return number1 + number2;
	}

	public int multiply() {
		return number1 * number2;
	}

	public void doubleValue() {
		this.number1 *= 2;
		this.number2 *= 2;
	}

}
```
---
### /src/com/in28minutes/primitive/datatypes/BiNumberRunner.java

```java
package com.in28minutes.primitive.datatypes;

public class BiNumberRunner {

	public static void main(String[] args) {
		BiNumber numbers = new BiNumber(2, 3);
		
		System.out.println(numbers.add());//2+3
		System.out.println(numbers.multiply());//2*3
		
		numbers.doubleValue();//Double both numbers 
		
		System.out.println(numbers.getNumber1());//4
		System.out.println(numbers.getNumber2());//6
	}

}
```
---