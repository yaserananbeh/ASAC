# HTML Links, CSS Layout, JS Functions Reading notes

# Links 

We can display link using the a tag in html

        <a href=" Url or path"  >The Message that will show in our page</a>

We can use links to redirect us to :
 - another website  `<a href="https://www.google.com"></a>`
 - to another page in the same website `<a href="./js/main.js"></a>`
 - Email links `<a href="mailto:yaser@example.com"></a>`
 - link to specific element on the same page `<a href="#id"></a>`

We can make the link open in new window using this attribute `target = "_blank" `

Link to the element in the same page by adding id to the element then put hash and the id in the href attribute


# Layout

        how to control where each element sits on a page and how to create attractive page layouts.


## Key Concepts in Positioning Elements

### Building Blocks
CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.

 - Block-level boxes start on a new line and act as the main building blocks of any layout, while inline boxes flow between surrounding text.
 - You can control how much space each box takes up by setting the width of the boxes (and sometimes the height, too). To separate boxes, you can use borders, margins, padding, and background colors .
 - Block-level elements : start on a new line Examples include: `<h1> <p> <ul> <li>`

 - Inline elements : flow in between surrounding text Examples include:<img> <b> <i>


 ### Containing Elements

 - If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element .
 - It is common to group a number of elements together inside a <div> (or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and the main navigation) .
 - The <div> element that contains this group of elements is then referred to as the containing element .Controlling the Position of Elements


 ### Controlling the Position of Elements

 - CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning.
 - You specify the positioning scheme using the position property in CSS. You can also float elements using the float property.
 - Normal flow
    Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.

 - Relative Positioning
    This moves an element from theposition it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed.

 -  Absolute positioning
    This positions the element in relation to its containing element. It is taken out of normal flow


NOTE To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed.

## Fixed Positioning
    This is a form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element. Elements with fixed position ingdo not affect the position of surrounding elements and they do not move when the user scrolls up or down the page

## Floating Elements
    allows you to take that element out of normal flow and position it to the far left or right of a containing box. The floated element becomes a block-level element around which other content can flow.

> When you move any element from normal flow, boxes can overlap. The z-index property allows you to control which box appears on top.

 ## Normal Flow
- position:static
In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax would be: position: static;

- position:relative
moves an element in relation to where it would have been in normal flow. For example, you can move it 10 pixels lower than it would have been in normal flow or 20% to the right.

- position:absolute
When the position property is given a value of absolute,the box is taken out of normal flow and no longer affects the position of other elements on the page.

- position:fixed
is a type of absolute positioning that requires the position property to have a value of fixed. It positions the element in relation to the browser window. Therefore, when a user scrolls down the page, it stays in the exact same place.



## Overlapping Elements
`z-index`

        If you want to control which element sits on top, you can use the z-index property. Its value is a number, and the higher the number the closer that element is to the front. For example, an element with a z-index of 10 will appear over the top of one with a z-index of 5.



## Floating Elements
        float The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible. Anything else that sits inside the containing element will flow around the element that is floated.



## Screen Sizes
        Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.

# Functions, Methods, and Objects

## Functions
let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).

## DECLARING A FUNCTION
FUNCTION KEYWORD FUNCTION NAMe function sayHello() { document.write(‘Hello!’);}

## CALLING A FUNCTION
FUNCTION NAME sayHello();

## VARIABLE SCOPE
The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable’s scope.

## VARIABLE SCOPE
The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable’s scope.

## GLOBAL VARIABLES
If you create a variable outside of a function, then it can be used anywhere within the script. It is called a global variable and has global scope.