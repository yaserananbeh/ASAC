## Class 03
## Passing Functions as Props

### What does .map() return?
**It returns new array that contain the same number of elements that the original array has**
### If I want to loop through an array and display each value in JSX, how do I do that in React?
**We can use the map method to loop through the array and return an html or jsx element**
### Each list item needs a unique ____.
**Key**
### What is the purpose of a key?
**in order to make a unique number that every element we render has to make the react distinguish between**


### What is the spread operator?
**The spread operator is a new addition to the set of operators in JavaScript ES6. It takes in an iterable (e.g an array) and expands it into individual elements.The spread operator is commonly used to make shallow copies of JS objects. Using this operator makes the code concise and enhances its readability.**

### List 4 things that the spread operator can do.
 - Copying an array
 - Concatenating or combining arrays
 - Using Math functions
 - Using an array as arguments
### Give an example of using the spread operator to combine two arrays.
```
const myArray = [`0`,`1`,`2`]
const yourArray = [`3`,`3`,`4`]
const ourArray = [...myArray,...yourArray]
```
### Give an example of using the spread operator to add a new item to an array.
```
const arr1 = ['9','10','20']
const  arr2= ['2', '5', ...fewFruit]
```
### Give an example of using the spread operator to combine two objects into one.
```
const objectOne = {hello: "hey"}
const objectTwo = {world: "Man"}
const objectThree = {...objectOne, ...objectTwo, laugh: "hhhh"}
```



### In the video, what is the first step that the developer does to pass functions between components?
 - make a function that change the state and pass it as a props to the another component to fire it from there 

### In your own words, what does the increment function do?
 - mapping through the array which is exist inside the component state and add one to the count of the matching name then set the state again with the new array that the map return
### How can you pass a method from a parent component into a child component?
- using the props we can pass anything properties or function 
### How does the child component invoke a method that was passed to it from a parent component?
with calling this.props then the name of the function key that we have already pass it from the other component 