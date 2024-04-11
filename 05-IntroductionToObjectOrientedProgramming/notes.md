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
    