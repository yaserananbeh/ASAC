## Class 03
## Java Primitives versus Objects

**Java has a two-fold type system consisting of primitives such as int, boolean and reference types such as Integer, Boolean. Every primitive type corresponds to a reference type**

### the differences between them : 
- regarding to the momery 
  
    - primitive

            boolean – 1 bit
            byte – 8 bits
            short, char – 16 bits
            int, float – 32 bits
            long, double – 64 bits

    - wrapper classes

            Boolean – 128 bits
            Byte – 128 bits
            Short, Character – 128 bits
            Integer, Float – 128 bits
            Long, Double – 192 bits
- regarding to the performance 
            
            the class wrapper slower than using the primitive types 

- regarding the usage 

        the primitive types are much faster and require much less memory. Therefore, we might want to prefer using them.
        On the other hand, current Java language specification doesn't allow usage of primitive types in the parametrized types (generics),  in the Java collections or the Reflection API.
**in conclusion the using the primitive types is much faster than the objects but on some cases we the primitive types don't work so we will choose the wrapper classes instead**

## Exceptions in java 
**Definition**: An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions.

**the valid java program must have an exceptions using the try statement or using the throws method**

### Three Kinds of Exceptions:
- the checked exception: like handling the un expect input from the users
- the error: if something wrong happened related to the hardware or system malfunction.
- runtime exception: These usually indicate programming bugs, such as logic errors or improper use of an API


## Scanning
**We use them to get inputs from the user, and objects of type Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.**

**Here's an example of how to make scanner**
```public static void main(String[] args) {
    Scanner myObj = new Scanner(System.in);

    System.out.println("Enter name, age and salary:");

    // String input
    String name = myObj.nextLine();

    // Numerical input
    int age = myObj.nextInt();
    double salary = myObj.nextDouble();

    // Output input by user
    System.out.println("Name: " + name);
    System.out.println("Age: " + age);
    System.out.println("Salary: " + salary);
  }
  ```
  - the example above show us that we in order to use the scanner we have to make an instance from it 
  - and then print out a message to the users to enter the entries 
  - then we can save the entries inside a variable using the instance.nextLine();
  - after that we can work with the accepted data as we would like 