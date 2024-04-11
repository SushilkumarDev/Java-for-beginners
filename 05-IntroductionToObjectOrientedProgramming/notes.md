# Big Picture - Thinking Objects
- We are used to thinking about things in the real world perspective. When we think about a flight that I would need to take from Hyderabad to NewYork, I would start thinking about what are all things that are involved! Tickets, Airport, Airlines, Check-In Counter, Flights, Passengers, AirHostess etc!
- We think a little differently when we used to design structured programs with C or Pascal. We think about things that we need to do, the data that we need to them and organize them into methods. Focus is on identifying the methods.
    
    //Thinking in terms of structured programming - methods
    fly() {

      //All data is here
      
      travelToAirport();
      findCheckInCounter();
      checkIn();
      passSecurityCheck();
      waitForBoardingCall();
      boardTheFlight();
      wishTheAirHostess();
      takeOff();
      haveFun();
      landing();
    }

  - Object Oriented Programming 
    - You start thinking in terms of objects

    CabService
        bookCab()
    
    Cab
        on()
        off()
        drive()
        reverse()
    
    SecurityCheck
      execute()
    
# Aim
Build a Motor Bike class with capabilities to adjust speed and gears.  We would want to create two objects honda and ducati and play with them. 
- Understand concepts of Class, Object, State, Behavior

Person is a class. Mahatma Gandhi and Nelson Madela are instances of a Class - objects.

- Concepts
  - Object Oriented Program is a bunch of objects sending messages to each other.
  - Important Concepts are Object, Class, State (How do we represent state?) and Behavior
  - Object
    - Has a Type or Class
    - Made up of other objects
    - Has an interface
      - Defines what messages it can receive 

> Instead of Bike, directly create MotorBike.

> Create seperate Runner classes where possible.

\com\in28minutes\program1\Planet.java
```
package com.in28minutes.program1;

//Question Answered : What is Class? What is Object?

public class Planet 
{
	// name
	// distance from sun

	public static void main(String[] args) {
		Planet earth = new Planet();
		Planet mars = new Planet();
		Planet venus = new Planet();
	}
}

public class MotorBike {

}

MotorBike ducati = new MotorBike();
MotorBike honda = new MotorBike();

Exercises 
- Create another instance of Planet.
- Create another instance of MotorBike.
- Create a new class called Book and create three instances
	- Art Of Computer Programming
	- Effective Java
	- Clean Code

```