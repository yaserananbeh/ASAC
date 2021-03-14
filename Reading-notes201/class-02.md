# Basics of HTML, CSS & JS


## tags to control Text


Headings we use them to show the importance of the data which we need to display in our pages
``
        <h1>
        <h2>
        <h3>
        <h4>
        <h5>
        <h6>        
``


Paragraphs
        `<p>`


Bold & Italic
        `<b>` and `<i>`

Superscript & Subscript
        `<sup>` and `<sub>`

Line Breaks & Horizontal Rules 
        `<br> and <hr>`


Strong & Emphasis
        `<strong>` and `<em>`


Quotations
            `<blockquote>` used for longer quotes that take up an entire paragraph.
            `<q>` element is used for shorter quotes that sit within a paragraph.


abreviations & Acronyms
            `<abbr title="Professor">Prof</abbr>`

Citations & Definitions
            `<cite>` element can be used to indicate where the citation is from.

Author Details
            `<address>` 

Changes to Content
              `  <ins>    <s>     <del>`

## Semantic Markup
        some text elements that are not intended to affect the 
        structure of your web pages, but they do add extra information to the 
        pages 




## CSS introduction

**Example Styles** That we can controll using the css 
 - Boxes
    - Width and height
        Borders (color, width, and style)
        Background color and images
        Position in the browser window.
 - Text
    - Typeface
        Size
        Color
        Italics, bold, uppercase,
        lowercase, small-caps
 - Specific
    - There are also specific ways
        in which you can style certain
        elements such as lists, tables,
        and forms.

## CSS works by associating rules with HTML elements.
 These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration.

**Selectors** 
indicate which
element the rule applies to.
The same rule can apply to
more than one element if you
separate the element names
with commas.

**Declarations**
indicate how
the elements referred to in
the selector should be styled.
Declarations are split into two
parts (a property and a value),
and are separated by a colon.

CSS declarations sit inside curly brackets and each is made up of two
parts: a property and a value, separated by a colon. You can specify
several properties in one declaration, each separated by a semi-colon.

**Properties** 
 indicate the aspects
of the element you want to
change. For example, color, font,
width, height and border.

**Values**
 specify the settings
you want to use for the chosen
properties. For example, if you
want to specify a color property
then the value is the color you
want the text in these elements
to be.

## We can use the css by three way on our html file
 - inline by define the style and assign what we need inside to same tag like `<p style="color: red";></p>`
 - or we can define style tag on the head of the file above the body tag like 
    ```
    <style>
        p{
            color: red;
        }
    </style>
    ```
 - also we can link our Html file with another css external file using link we put it on the head like 
 ```
 <link rel="stylesheet" href="THE PATH OF OUR CSS FILE">
 ```

### Why use usually External Style Sheets?
- All of your web pages can share the same style sheet. mean we don't need to repeat the code on each html page
- once the user has downloaded the CSS stylesheet, the rest of the site will load faster. If you want to make a change to how your site appears, you only need to edit the one CSS file and all of your pages will be updated.
- It is generally considered good practice to have the content of the site separated from the rules that determine how it appears.

## Here I will provide the type of selectors that we use in the css 
- Universal Selector

            Applies to all elements in the document Example : ```*{    }```
- Type Selector

            Matches element names Example : h1, h2, h3 {}

- Class Selector

            Matches an element whose
            class attribute has a value that
            matches the one specified after
            the period (or full stop) symbol Example : .note {}
- ID Selector

            Matches an element whose
            id attribute has a value that
            matches the one specified after
            the pound or hash symbol Example : #introduction {}
- Child Selector

            Matches an element that is a
            direct child       Example :   li>a {}    
- Descendant Selector

            Matches an element that is a
            descendent of another specified
            element (not just a direct child of
            that element) Example : p a {}
- Adjacent Sibling Selector

            Matches an element that is the
            next siblin         Example : h1+p {}
- General Sibling Selector

            Matches an element that is a
            sibling of another, although it
            does not have to be the directly
            preceding element Example : h1~p {}


## javascript 

COMMENTS `/*  multi line comment */`  and `// to define single line comment ` 

### WHAT IS A VARIABLE? 
        A container to store a value which is changable to a specfic name

        We can define the variables by use VAR OR LET OR CONST THEN the name of the variable then the assignment value after equal sympol

### Data types 
        String , Integer , boolean , float 

### ther's some rules for naming variables
 - must not start with number 
 - don't use dashes and dotes 
 - don't use the reserved keywords 
 - case sensitive 
 - use name that descibe the variable content 
 - use camel case 


## arrays 
the array look like the job of the variables but the array can store more than one value with the same name
we use it when we need to store group of data that related with each other 

        var colors; 
        colors = ['white', 'black', ' custom']; 


We can reach any array element using his index and also we can know the number of elements which it inside the array by using array.length

The indexes in the array start from zero as I said before we can use the index to find the element value and we can change it as well 


arithmetic operators 
` + - * / ++ -- % `


## Decisions and loops 

We use them to control the code flow and to control code run times 

Example of the decisions ( If , switch )

Examples about the loops (for , while , do while , for each);


## comparision operator
we using it to compare two values and the result of those operators is True or False some example of those operator

`==` Is equal to This to sure if the two sides before and after is equal each other then will return true if not equal will return false

`!=` Is not equal this to be sure if the two sides is not equal eathother, return true if is not and return false if equal each other

`===` to be sure if the two sides of arround the operator is equal each other in value and datatype

`!==` to be sure if the two sides are not equal in the value and in the data type as well.

`>` Greater than

`<` less than

`<=` less than or equal to

`>=` greater than or equal to

### The main difference between for and while
in for we use it usually with the numbers and we should know the End of the loop
in while it is more efficient with the strings and we use with the cases that we don't how many the code will run