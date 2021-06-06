## Class 02
## State and Props

### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?
**The render before the componentDidMount**

### What is the very first thing to happen in the lifecycle of React?
**the constructor is the first thing will happen**

### Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
1. constructor
2. render()
3. componentDidMount()
4. React Updates
5. componentWillUnmount



### componentDidMount
 is executed after the first render only on the client side. This is where DOM or state updates should occur. This method is also used for integration with other JavaScript frameworks and any functions with delayed execution such as setTimeout or setInterval. We are using it to update the state so we can trigger the other lifecycle methods.


### What types of things can you pass in the props?
can be any data type, from strings to functions, objects, etc.

### What is the big difference between props and state?
the props to pass the data into a component but the state is handled inside the component 
### When do we re-render our application?

### What are some examples of things that we could store in state?
when we need to handle changes from the user or the forms 
