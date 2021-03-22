# Forms and Events

## Forms
The forms the container that make the users able to put any type of data and we can dealing with data to make our website more dynamic and interactive with any types of users 

there's more than one type of control that we can use to collect information from the user 

- form part to fetch the text data like 
  - text input 
  - password input 
  - text area 
- Making choices 
  - checkboxes 
  - radio buttons 
  - dropdown boxes 
- submitting forms by : 
  - image 
  - submit buttons 

- uploading files
  - file upload 

To define a form in our page we use the `<form>` tag and this openning tag should contains two attributes : the action where the form will redirect us after submitting it and the second attribute is the method which can be get or post

### the controls 
- input type text make a text field 
- input type password make a password field
- textarea make a text area and we can include multi line text in it 
- input type radio to display a choice button this tag can contains value , name , checked attributes 
- input type checkbox to display a choice but this type we can choose more than one choice 
- select tag to display a dropdown in our page the inner tags is option
- input type file to make the user able to attach a file 
- input type submit this make us able to send the form data by get or post method and redirect us to the new target which we mentioned before in the form action property 
- input type image we can use it like a submit button 
- button we use it like the ancher tag and we use it to be more flexible to add an image with text between the openning tag and closing tag 
- label we use this type to labeling the form controls like the discription of the next form control 
- fieldset to group the form controls together and the legend inside it to naming the group with specific title
- input date to display a field that should contain a date form only 
- input type email to be sure the input information contain email form (example@a.com)
- input type search 


## Lists, Tables & Forms”

- we can control the type of ordered-unordered Lists bullets using list-style-type(none , disc , circle, square, decimal, decimal-leading-zero, lower-alpha , upper-alpha, lower-roman, upper-roman ) also we can use image instead all of these types 
- we can control the position of these bullets using this attributes list-style-position (outside or inside )
- table properties (width , padding , text-transform to convert the data to uppercase, letter-spacing , font-size , border-top,border-bottom, text-align , background-color, :hover)
- also we can edit the empty cells (show, hide , inherit) and porder-spacing , border-collaps to control the spaces between the cells 
- we can style the form controls style text inputs (font-size, color , background-color, border , border-radius , :focus, :hover, background-image) and the submit button(color, text-shadow, border-bottom, background-color , : hover ) and these attributes we can use them as well for the fieldset
- we can change the type of the cursor to be (auto , crosshair, default , pointer, move , text , wait , help ,url("example.gif"))


### Events 

There's a three ways to bind an event to an element 
- html Element Handler (bad practice to use it )
- Dom event handler `element .onevent functionName ;`
- Event listeners `element .addEventlistener('event', functionName [, Boolean]) ;`
- Events are the browser's way of indicating when something has happened (such as when a page has finished loading or a button has been clicked). 
- Binding is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon. 
- When an event occurs on an element, it can trigger a JavaScript function. When this function then changes the web page in some way, it feels interactive because it has responded to the user. 

- You can use event delegation to monitor for events that happen on all of the children of an element.
