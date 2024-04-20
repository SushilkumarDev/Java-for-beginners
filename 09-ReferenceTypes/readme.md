## Reference Types 

- Reference Variables vs Primitive Variables
  - memory
  - assignment
  - initialization (null)

- Predefined Reference Types in Java
  - String
  - Wrapper Classes
  - LocalDate, LocalDateTime

### Reference Variables

- What are Reference Variables?
- How are they stored in memory?
- How are they initialized?
- How does assignement and equality work with Reference Variables

```
Animal dog = new Animal();
```

The instance of new Animal - Animal object - is created in memory. The memory address of the object created is stored in the dog reference variable.

Reference Variables contains a reference or a guide to get to the actual object in memory.

#### Puzzles

```
Animal dog1 = new Animal();
dog1 = new Animal();
```

What will happen?

Two objects of type Animal are created. Only one reference variable is created.

```
Animal animal1 = new Animal();
Animal animal2 = new Animal();
animal1 = animal2;
```

What will happen? What would happen if the same was done with primitive variables?

#### == (equals) operator
- Equality for Primitives only compares values
- For reference variables, == compares if they are referring to the same object.

```
int a = 5;
int b = 5;
System.out.println(a == b);//true
```

```
Integer aReference = new Integer(5);
Integer bReference = new Integer(5);

System.out.println(aReference == bReference);//false

bReference = aReference;

//Now both are referring to same object
System.out.println(aReference == bReference);//true
```
### String Class
- A String class can store a sequence of characters. 
- String is not a primitive in Java but a Class in its own right.


```
//Get Data From String
"This is a piece of Text".length()

//Get Characters from String
str.charAt(0)
str.charAt(1)
str.charAt(20)
str.charAt(22)
str.charAt(-22)

//Get Substring from String
str.substring(11)
str.substring(11, 15)

//Searching Content of a String
str.indexOf('C')
"test".indexOf("te")
str.lastIndexOf('C')
"test".lastIndexOf("te")

//Checking Content of a String
str.equalsIgnoreCase("test");
str.contains("ABCD");
str.endsWith("78")
str.startsWith("01");
str.isEmpty();
```