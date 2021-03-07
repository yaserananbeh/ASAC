# Dynamic Web Pages with CSS
## Here I will put my notes about the Design Web Pages with CSS topic from Read 06b

## CSS introduction

## What is the css 
Css stands for Cascading Style Sheets CSS allows you to create rules that specify how the content of
an element should appear. For example, you can specify that
the background of the page is cream, all paragraphs should
appear in gray using the Arial typeface, or that all level one
headings should be in a blue, italic, Times typeface.

### **Here some examples about the block and inline element in html**

**Block level elements**


look like they start on a new line. Examples include the `<h1>-<h6>, <p> and <div>` elements.

**Inline elements**

flow within the text and do not start on a new line. Examples include `<b>, <i>, <img>, <em> and <span>`

Note Everyone of these elements have a border aroud it but we can't control with this feature to appeare without the css
    
    CSS allows you to create rules that control the way that each individual box (and the contents of that box) is presented.

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

