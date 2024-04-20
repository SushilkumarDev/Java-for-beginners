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

## String Puzzles

- Modification of a String 
- Strings are immutable. Value of a String Object once created cannot be modified. Any modification on a String object creates a new String object.

```
String str3 = "value1";
str3.concat("value2");
System.out.println(str3); //value1
str.toLowerCase()
str.toUpperCase()
"012301230123".replace('0', '4')
" abcd  ".trim()
```

String Concatenation Operator
- RULE1: Expressions are evaluated from left to right.
    - Except if there are parenthesis.
- RULE2: number + number = number
- RULE3: number + String = String

```
System.out.println(5 + "Test" + 5); //5Test5
System.out.println(5 + 5 + "Test"); //10Test
System.out.println("5" + 5 + "Test"); //55Test
System.out.println("5" + "5" + "25"); //5525
System.out.println(5 + 5 + "25"); //1025
System.out.println("" + 5 + 5 + "25"); //5525
System.out.println(5 + (5 + "25")); //5525
System.out.println(5 + 5 + 25); //35
```

#### String vs StringBuffer vs StringBuilder
- Immutability : String
- Thread Safety : String(immutable), StringBuffer

### Wrapper Classes

#### What are Wrapper Classes?

- A wrapper class wraps (encloses) around a data type and gives it an object appearance
- Wrapper classes are final and immutable.

Types
- Wrapper: Boolean,Byte,Character,Double,Float,Integer,Long,Short 
- Primitive: boolean,byte,char ,double, float, int , long,short


#### Why Wrapper Classes?

Creation from other data types

```java
Integer hundred = Integer.valueOf("100");
Boolean value = Boolean.valueOf("True");
```

Utility Methods

```
//Conversion

Float floatWrapper = Float.valueOf(57.0f);
int floatToInt = floatWrapper.intValue();//57

Integer seven = 
    Integer.valueOf("111", 2);

Integer.toString(seven, 2);

```

Storing into a collection


#### Creation of Wrapper Classes

Prefer valueOf instead of Constructors!

```
Integer seven = 
    Integer.valueOf("111", 2);//binary 111 is converted to 7

Integer hundred = 
    Integer.valueOf("100");//100 is stored in variable
```


```
Integer number = new Integer(55);//int
Integer number2 = new Integer("55");//String

Float number3 = new Float(55.0);//double argument
Float number4 = new Float(55.0f);//float argument
Float number5 = new Float("55.0f");//String

Character c1 = new Character('C');//Only char constructor
//Character c2 = new Character(124);//COMPILER ERROR

Boolean b = new Boolean(true);

//"true" "True" "tRUe" - all String Values give True
//Anything else gives false
Boolean b1 = new Boolean("true");//value stored - true
Boolean b2 = new Boolean("True");//value stored - true
Boolean b3 = new Boolean("False");//value stored - false
Boolean b4 = new Boolean("SomeString");//value stored - false

b = false;

```

#### Convert Wrappers to Primitives

xxxValue methods help in creating primitives

```
Integer integer = Integer.valueOf(57);
int primitive = seven.intValue();//57
float primitiveFloat = seven.floatValue();//57.0f

Float floatWrapper = Float.valueOf(57.0f);
int floatToInt = floatWrapper.intValue();//57
float floatToFloat = floatWrapper.floatValue();//57.0f
```