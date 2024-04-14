<!---
Current Directory : /in28Minutes/git/java-a-course-for-beginners/7-Conditionals
-->

## Complete Code Example


### /src/com/in28minutes/ifstatement/examples/IfStatementRunner.java

```java
package com.in28minutes.ifstatement.examples;

public class IfStatementRunner {

	public static void main(String[] args) {
		puzzle5();
	}

	private static void puzzle1() {
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
		
	}
    	private static void puzzle2() {
		int l = 15;

		if (l < 20)
			System.out.println("l<20");//
		if (l > 20)
			System.out.println("l>20");
		else
			System.out.println("Who am I?");//
	}

	
	
	private static void puzzle3() {
		int m = 15;

		if(m>20) 
		    if(m<20)
		System.out.println("m>20");
		    else
		System.out.println("Who am I?");
	}


	private static void puzzle5() {
		int number = 5;
		if(number < 0) 
		    number = number + 10; 
		number++; 
		System.out.println(number);
	}