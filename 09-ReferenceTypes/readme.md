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

