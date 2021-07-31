# Class-06 
# Inheritance and Interfaces

### review Objects and Classes
- Objects : are the main core of the oop programming, anything that we can see and interact with is an object (Dog , TV, ...) every object has states(fields) and behaviors(methods) 
**some of benefits to use the objects in the programming**
   Enhance the (Modularity,Information hiding, reusability and the Pluggability) 
- Classes : are the blueprints that make or create each individual object
- Inheritance : the way that object oriented allows classes to inherits commonly used states and behaviors
- Interface : provide an interaction with the object methods from outside and Implementing an interface allows a class to become more formal about the behavior it promises to provide. Interfaces form a contract between the class and the outside world, and this contract is enforced at build time by the compiler. If your class claims to implement an interface, all methods defined by that interface must appear in its source code before the class will successfully compile.
- Package : is a namespace that organizes a set of related classes and interfaces, Because software written in the Java programming language can be composed of hundreds or thousands of individual classes, it makes sense to keep things organized by placing related classes and interfaces into packages.

## Summary of Interfaces 
- An interface declaration can contain method signatures, default methods, static methods and constant definitions. The only methods that have implementations are default and static methods.

- A class that implements an interface must implement all the methods declared in the interface.

- An interface name can be used anywhere a type can be used.

## Summary of Inheritance
Except for the Object class, a class has exactly one direct superclass. A class inherits fields and methods from all its superclasses, whether direct or indirect. A subclass can override methods that it inherits, or it can hide fields or methods that it inherits. (Note that hiding fields is generally bad programming practice.)

The table in Overriding and Hiding Methods section shows the effect of declaring a method with the same signature as a method in the superclass.

The Object class is the top of the class hierarchy. All classes are descendants from this class and inherit methods from it. Useful methods inherited from Object include toString(), equals(), clone(), and getClass().

You can prevent a class from being subclassed by using the final keyword in the class's declaration. Similarly, you can prevent a method from being overridden by subclasses by declaring it as a final method.

An abstract class can only be subclassed; it cannot be instantiated. An abstract class can contain abstract methods—methods that are declared but not implemented. Subclasses then provide the implementations for the abstract methods.
