# Object-Oriented Programming, HTML Tables

## Domain Modeling 
The domain modeling is creating a conseptual model in the code for specific problem 

Here's some tips to follow when building domain models.

- When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
- Model its attributes with a constructor function that defines and initializes properties.
- Model its behaviors with small methods that focus on doing one job well.
- Create instances using the new keyword followed by a call to a constructor function.
- Store the newly created object in a variable so you can access its properties and methods from outside.
- Use the this variable within methods so you can access the object's properties and methods from inside.


## Tables

A table represents information in a grid format. 
Examples of tables include financial reports, TV schedules, and sports results.

- The `<table>` element is used to add tables to a web 
page.
-  A table is drawn out row by row. Each row is created 
with the `<tr>` element.
-  Inside each row there are a number of cells 
represented by the `<td>` element (or `<th>` if it is a 
header).
-  we can make cells of a table span more than one row 
or column using the rowspan and colspan attributes.
-  For long tables you can split the table into a `<thead>`, 
`<tbody>`, and `<tfoot>`.
- we can control the table's border and background 

#### Table code example 

        <html>
        <head>
        <title>Tables</title>
        </head>
        <body>
        <table>
        <thead>
        <tr>
        <th></th>
        <th scope="col">Home starter hosting</th>
        <th scope="col">Premium business hosting</th>
        </tr>
        </thead>
        <tbody>
        <tr>
        <th scope="row">Disk space</th>
        <td>250mb</td>
        <td>1gb</td>
        </tr>
        <tr>
        <th scope="row">Bandwidth</th>
        <td>5gb per month</td>
        <td>50gb per month</td>
        </tr>
        <!-- more rows like the two above here -->
        </tbody>
        <tfoot>
        <tr>
        <td></td>
        <td colspan="2">Sign up now and save 10%!</td>
        </tr>
        </tfoot>
        </table>
        </body>
        </html>

## Functions, Methods, and Objects

the function is a block of code has a name and when we call it name we execute it code 
and the function has a return keyword to specify what the fuction will return when we call it 

Method is the same like the functions but usually the method will be a function which inside an object and we can call it using the name of the object then dot then the function name with perantheses 

object every element or every data type in javascript is object the object is like the array it can contain more than one properties but the object can hold the methods also 

the constructur object is an object but it name start with capital letter and we can make how many copy we want by make a variable and assign the name of the object with NEW keyword before the name this will make a copy of the object and then we can add properties and method to it or change its internal data by call the name of the variable and add dot then the property name or the method name then and assign the values 

#### we can make an object more than one way 
- object litrals 
- using the newObject() method then assign the properties and methods to it using  dot 


### this keyword
we use it to mention to the object name usually we use it inside the method to refer the object name that contain this method


## summary

- Functions allow you to group a set of related statements together that represent a single task. 
- Functions can take parameters (informatiorJ required to do their job) and may return a value. 
- An object is a series of variables and functions that represent something from the world around you. 
- In an object, variables are known as properties of the object; functions are known as methods of the object. 
- Web browsers implement objects that represent both the browser window and the document loaded into the browser window. 
- JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts. 
- Arrays and objects can be used to create complex data sets (and both can contain the other). 