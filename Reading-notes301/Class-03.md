## Class 02


# Lists

- In React, transforming arrays into lists of elements is nearly identical.
- we can build collections of elements and include them in JSX using curly braces {}.

# Keys

- Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

- The best way to pick a key is to use a string that uniquely identifies a list item among its siblings

- Keys only make sense in the context of the surrounding array.

- Keys used within arrays should be unique among their siblings

# Spread syntax
- allows an iterable such as an array expression or string to be expanded in places where zero or more arguments (for function calls) or elements (for array literals) are expected, or an object expression to be expanded in places where zero or more key-value pairs (for object literals) are expected

# How to Pass Functions between Components
- we can pass functions from one component to another. We do this because the functions that control one components state have to reside in the same component as the state. So, if one component needs to update the state of another then it needs to have the function from the first component.

- here the code that explain how to make that between two component their names are Person and App

App.js

```
import React, { Component } from 'react';
import Person from './Person';
import './App.css';
// 
class App extends Component {
    
    constructor(){
        super();
        this.state = {
            people: [
                {name:'Bob', count: 0},
                {name:'Tina', count: 0},
                {name:'Louise', count: 0},
                {name:'Linda', count: 0},
                {name:'Gene', count: 0}
            ]
        }
    }
    
    increment = (name) => {
        let ppl = this.state.people.map( (p) => {
            if(p.name === name){
                p.count++;
            }
            return p;
        });
        this.setState({people: ppl});
    }
    
    render() {
        return (
          <div className="App">
            {this.state.people.map( (person) => (
                <Person name={person.name} 
                        key={person.name} 
                        count={person.count} 
                        increment={this.increment}/>
            ))}
          </div>
        );
    }
}

export default App;


```

Person.js

```
import React, {Component} from 'react';

export default class Person extends Component{
    
    constructor(props){
        super(props);
        this.state={
            hasChanged: false
        }
    }
    
    increment = (ev) => {
        ev.preventDefault();
        this.setState({hasChanged:true});
        
        this.props.increment(this.props.name);
    }
    
    render(){
        return (
            <div className="person">
                <h2>{this.props.name}</h2>
                <h3>{this.props.count}</h3>
                <button onClick={this.increment}>Add</button>
                {this.state.hasChanged && (
                    <span>Updated</span>
                )}
            </div>
        );
    }
}


```