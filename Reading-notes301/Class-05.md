# Class-05

### How would you break a mock into a component heirarchy?
- we can do that when we convert every UI part to a component then we will get a components that contain other
### What is the single responsibility principle and how does it apply to components?
The single-responsibility principle (SRP) is a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part. All of that module, class or function's services should be narrowly aligned with that responsibility.
### What does it mean to build a ‘static’ version of your application?
- build a version that takes your data model and renders the UI but has no interactivity
### Once you have a static application, what do you need to add?
build components that reuse other components and pass data using props
### What are the three questions you can ask to determine if something is state?

1. Is it passed in from a parent via props? If so, it probably isn’t state.
2. Does it remain unchanged over time? If so, it probably isn’t state.
3. Can you compute it based on any other state or props in your component? If so, it isn’t state.

### How can you identify where state needs to live?

- Identify every component that renders something based on that state.

- Find a common owner component

- Either the common owner or another component higher up in the hierarchy should own the state.

- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

