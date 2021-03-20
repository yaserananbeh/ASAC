# Problem Domain, Objects, and the DOM

## Understanding the problem domain is the hardest part of programming

 * understanding the problem domain is the hardest part of programming, according to programming experts. In a Pluralsight course, the "Protein Tracker" app is an example of a simple app that is easily understood. By creating a familiar problem domain, we can make teaching and learning easier, says Mark Johnson. It also provides a reference problem domain that doesn't have to be re-learned, he says. It provides a way to compare and contrast different technologies, and it's free if the viewer has already watched one of our other courses.

* Writing code is a lot like putting together a jigsaw puzzle. Programming is easy if you understand the problem domain. Many problem domains are like a puzzle with a blurry picture or no picture at all. When writing code, we put together code with the purpose of building components that we have taken out of the "bigger picture" of the problem Domain is a problem domain that needs to be understood before writing code. It's a problem that can only be solved by understanding the problem.

* If understanding the problem domain is the hardest part of programming, you can do one of two things to make it easier. Cut out cases and narrow your focus to a particular part of the problem. The other choice is to become better at understanding problem domains. I'm still not ready to unveil exactly what I am building, but I do have an active mailing list where you can sign up to find out when I release the product I'm working on.

## Document Object Mode

- The browser shows a DOM tree tab. 
- There are four types of nodes in DOM trees: document nodes, Nodes of part, nodes of attributes and nodes of text. 
- You can use their id or cl ass to pick element nodes 

- Tag Name or CSS selector syntax of attributes. 

- Any time a DOM question returns more than one Node, always a Nadel I st will come back. 

- You can view and update an element node 
- Assets include textContent and content 
- I nnerHTML or use techniques for DOM manipulation. 
- A node element may include several text nodes and The elements of children who are mutually siblings.
- The implementation of the DOM is in older browsers Incompatible (and is a popular reason for using jQuery). 
- Browsers include DOM tree display resources

### Note Each node is an object with methods and properties. Scripts access and update this DOM tree (not the source HTML file). Any changes made to the DOM tree are reflected in the browser. 


when we make any web page the browser will make a DOM for our page and make every element in the page as an object this object we can access to it by many ways the dom will provide many way to access them 

Example we can access any element by its ID using this command document.getElementById('the id') and this mean select the element which has this id and the type of dom return to us one element only(one node) like this command querySelector()

here another examples that return to us more than one element (nodeList) even if it only finds one element these command will return (nodeList) this nodelist will be has a number of indexes like the array and we can call the first element in the node by call the zero index of the node list examples to these command is `getElementsByTagName()` and `getElementsByClassName()` and `querySelectorAll()`


let's learn how to select an element from the node list after we select it : the first way is by using this command `document.getElementsByClassName('class').item(0)` this command select the first element in the node list which it returned from document.getElementsByClassName('class') and we can use the squer prackets enstead of the parnthesis and it's the best practise when we trying to reach an item in nodelist 

also we can use this command to reach more than one element in the dom `document.getElementsByTagName('li);` and this command `document.querySelectorAll('')` as well, this to select multiple element have the same css selector 

### Traversing the dom

    When you have an element node, you can select another element in relation to it using these five properties. This is known as traversing the DOM. 

- parentNode
- previousSibling
- nextSibling
- firstChild 
- lastChild
    ```    
        var startltem = document.getElementByid('two'); 
        var prevltem startltem.previousSibling; 
        var nextltem = startitem.nextSibling; 

        var startltem = document.getElementsByTagName('ul ') [OJ ; 
        var firstltem = startltem. firstChild; 
        var lastltem = startitem.lastCh i ld; 
    ```


