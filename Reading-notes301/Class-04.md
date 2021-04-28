# Class-04

# Forms
HTML form elements work a little bit differently from other DOM elements in React, because form elements naturally keep some internal state.

# controlled components

is a technique that handle the data that the user input in the forms like when we submit the form we should invoke like a handle function to handle the changes 

With a controlled component, the input’s value is always driven by the React state. While this means you have to type a bit more code, you can now pass the value to other UI elements too, or reset it from other event handlers.


# The Conditional (Ternary) Operator Explained


    person.driver = person.age >=16 ? 'Yes' : 'No';

the ternary operator:

    condition ? value if true : value if false

# here some important notes 

- The condition is what you’re actually testing. The result of your condition should be true or false or at least coerce to either boolean value.

- A ? separates our conditional from our true value. Anything between the ? and the : is what is executed if the condition evaluates to true.


- Finally a : colon. If your condition evaluates to false, any code after the colon is executed.

