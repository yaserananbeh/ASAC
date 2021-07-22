## Class 01
## Java Basics

**variables** the containers that hold information in the program to be referenced and manipulated

The Java programming language uses both "fields" and "variables" as part of its terminology. Instance variables (non-static fields) are unique to each instance of a class. Class variables (static fields) are fields declared with the static modifier; there is exactly one copy of a class variable, regardless of how many times the class has been instantiated. Local variables store temporary state inside a method. Parameters are variables that provide extra information to a method; both local variables and parameters are always classified as "variables" (not "fields"). When naming your fields or variables, there are rules and conventions that you should (or must) follow.

The eight primitive data types are: byte, short, int, long, float, double, boolean, and char. The java.lang.String class represents character strings. The compiler will assign a reasonable default value for fields of the above types; for local variables, a default value is never assigned. A literal is the source code representation of a fixed value. An array is a container object that holds a fixed number of values of a single type. The length of an array is established when the array is created. After creation, its length is fixed.

**Operators**
- assignment operator (=)
- arithmetic operators (+ - / * %)
- unary operators (+ - ++ --)
- Equality and Relational operators (== != > < >= <=)
- Conditional operators (&& || ?:)
- Bitwise and Bit Shift operators (~ << >> >>> & ^ | )
- Type Comparison operator (instanceof)

**Expressions, Statements, and Blocks**
- Expressions : a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value.
- Statements : a complete unit of execution
- Blocks : a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed

**Control Flow Statements**
The statements inside your source files are generally executed from top to bottom, in the order that they appear. Control flow statements, however, break up the flow of execution by employing decision making, looping, and branching, enabling your program to conditionally execute particular blocks of code. This section describes the decision-making statements (if-then, if-then-else, switch), the looping statements (for, while, do-while), and the branching statements (break, continue, return) supported by the Java programming language.


**compile code** means to make the code executable and the computer can execute it by converting the code to 1,0 machine language using another program 