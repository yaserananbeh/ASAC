# HTML Lists, Control Flow with JS, and the CSS Box Model

## Lists 

### there's three type of lists in html :

- **Ordered lists** are lists where each item in the list is numbered we use this tag : `<ol> which include a set of <li>`
- **Unordered lists** lists that begin with a bullet point  we use this tag : `<ul> which include a set of <li>`
- **Defintion lists**  are made up of a set of terms along with the definitions for each of those terms.
    we use these tags 
    `` <dl> the main tag to define the defintion list and we will see iside it a pairs of <dt> (the definition 
        term) and <dd> This is used to contain the 
        definition.``

### Note Lists can be nested inside one another and the browser will give another shape of bullets to the enternal lists 

## Boxes 

### Every element in html has a box hold it but let's take a look how to control them 

We can change the dimensions(size) of this box by adjusting the width and the height of it, also we can limiting the width by using these attributes (min-width & max-width ) and these to limiting the height of the box as well (min-height & max-height )

#### Overflowing Content overflow

using this we can make hide the extra content that doesn't fit the box size by using `overflow: hidden`
And this This property adds a scrollbar to the box so that users can scroll to see the missing content.by using `overflow: scroll`

### Borders 

We can control the width of the border, the style of the border and the color of the border , although we can control all of these border proparities with one command here example to figure out the shorthand of borders 
`border: 3px dotted #0088dd; first value for the width then the style then the color `

### Padding

allows us to specify how much space should appear between the content of an element and its border. 

        padding: 10px 5px 3px 1px;

### Margin 

we use this property to controls the gap between boxes

        margin: 1px 2px 3px 4px;
        margin: 10px 20px;


### Centering Content

        If you want to center a box on the page (or center it inside the element that it sits in), you can set the left-margin and right-margin to auto.
        and edit the width of the box 


### Change Inline/Block Display

 - inline
    - This causes a block-level element to act like an inline element.
 - block
    - This causes an inline element to act like a block-level element.
 - inline-block
    -  This causes a block-level element to flow like an inline element, while retaining other features of a        block-level element.
 - none
    - This hides an element from the page. In this case, the element acts as though it is not on the page at all 


### Visibility

We can control the visibility of the box by swap between `visibility : hidden` or `visibility : visible`

### box-shadow 
we can control the shadow that around our box using this proparity 
        `box-shadow: 5px 5px 5px 5px #777777;`
        
    the firs value to control the horizental offset the second to control the vertical offset the third to specify the blur distance and the last one to control the spread of shadow


### border-radius 

to control the angle amount of the border to make rounded corners 


# Javascript

### Variables 
As we know the defintion of the variables is a container to any type of data and can be changed 

**Decleration**

By using these keywords `var or let or const ` then enter the name of the variable don't forget the rules of naming the variables after the name we have to assign the variable value after equal sign 

**Data type**

the type of the data what we will assign to the variable maybe it will be a string or a number or a boolean 

we can use the variables to store any of these data types 

## **Decicions and loops**

### **Switch statment**

A switch statement starts with a variable called the switch value. Each case indicates a possible value for this variable and the code that should run if the variable matches that value. 

You have a default option that is run if none of the cases match. 
If a match is found, that code is run; then the break statement stops the rest of the switch statement running (providing better performance than multiple if statements)


### **Loops**

a type of statments or cammand that we can use them to control the flow of our code and for more explanation loops check a condition if the condition return true will do the same execution code how many time the condition ruturn true 

**Loops Examples**
 - for loop 
 - while 
 - do while 
 - foreach

 ### for loop 
 it will has 3 parts first one the initalization part and then the condition then the couter (update)

        for (var x=0 ; x<5; x++){
                // the execution code
        }

### while loop
it has 3 parts but a little bit different from the the for statment 

        var x=0;
        while (x < 5){
                //execution code 

                x++;
        }

### do while loop 
the same as the original while but it do the code for one time before it check the condition 

        var=0;
        do{
                //execution code 
                x++;

        } while(x<5);

        