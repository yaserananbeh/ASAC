# Class-05

## Thinking in React
- React is, in our opinion, the premier way to build big, fast Web apps with JavaScript. It has scaled very well for us at Facebook and Instagram.

- One of the many great parts of React is how it makes you think about apps as you build them. In this document, we’ll walk you through the thought process of building a searchable product data table using React.


## The mock like representation for how the data will look like and here an image to show the mock for json file 

![image]( https://reactjs.org/static/1071fbcc9eed01fddc115b41e193ec11/d4770/thinking-in-react-mock.png )

- and this the json api data
```
[
  {category: "Sporting Goods", price: "$49.99", stocked: true, name: "Football"},
  {category: "Sporting Goods", price: "$9.99", stocked: true, name: "Baseball"},
  {category: "Sporting Goods", price: "$29.99", stocked: false, name: "Basketball"},
  {category: "Electronics", price: "$99.99", stocked: true, name: "iPod Touch"},
  {category: "Electronics", price: "$399.99", stocked: false, name: "iPhone 5"},
  {category: "Electronics", price: "$199.99", stocked: true, name: "Nexus 7"}
];
```


# Break The UI Into A Component Hierarchy
-  The component hierarchy focuses the component’s scope of responsibility, creates meaningful relationships between components, encourages composability, and provides balance between flexibility and structure in our component library. This empowers external teams to build and evolve their UI more effectively and allows maintainers to more sustainably support them.

# Build A Static Version in React 
- To build a static version of any app that renders the data model, we want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. we don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, we don’t need it.


## Identify The Minimal (but complete) Representation Of UI State

To build your app correctly, you first need to think of the minimal set of mutable state that your app needs. The key here is DRY: Don’t Repeat Yourself. Figure out the absolute minimal representation of the state your application needs and compute everything else you need on-demand. For example, if you’re building a TODO list, keep an array of the TODO items around; don’t keep a separate state variable for the count. Instead, when you want to render the TODO count, take the length of the TODO items array.
Think of all of the pieces of data in our example application. We have:
The original list of products The search text the user has entered The value of the checkbox The filtered list of products Let’s go through each one and figure out which one is state. Ask three questions about each piece of data:
Is it passed in from a parent via props? If so, it probably isn’t state. Does it remain unchanged over time? If so, it probably isn’t state. Can you compute it based on any other state or props in your component? If so, it isn’t state.


# Where the State Should Live

- Identify every component that renders something based on that state.
- Find a common owner component (a single component above all the components that need the state in the hierarchy).
- Either the common owner or another component higher up in the hierarchy should own the state.
- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.