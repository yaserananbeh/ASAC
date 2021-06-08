# Class-04


### What is a ‘Controlled Component’?


    We can combine the two by making the React state be the “single source of truth”. Then the React component that renders a form also controls what happens in that form on subsequent user input. An input form element whose value is controlled by React in this way is called a “controlled component”.

### Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
    we should do update the state as soon as the user enter the data or change it becaues the setState function is async function

### How do we target what the user is entering if we have an event handler on an input field?
    set onChange event on the element that handle the changes and set it to the state properties


### Why would we use a ternary operator?
1. It always returns a value. JavaScript will throw a syntax error if only one expression is provided. 
2. It can save on multiple lines of code, without compromising readability.
### Rewrite the following statement using a ternary statement:
        if(x===y){
        console.log(true);
        } else {
        console.log(false);
        }


         (x===y)? console.log('true') : console.log('false');
