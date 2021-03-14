# Revision  Html & JavaScript introduction

## HTML 

HTML Stands for Hyper Text Markup Language which responsible to define the webpage Elements to be exist and show in our upcoming page 

Web prowser is the platform, Software   that show to the users the webpages 

Web server is the server that responsible to recieve the user request to fetch webpages then provide them to be able to show by the web browser

The screen reader that help us to show the content of webpages and it different from device to another

HTML Describes the Structure of Pages HTML Uses Elements to Describe the Structure of Pages

Every element in the html begin with openning tag and closing tag exept the self closing tag element 

The tag tell our browser what is the type of the element that we want to display on our webpage

every opening tag start with the angle pracket and then the name of the element then the right angle pracket 
like this 
`<p>test</p>`

We can put on the openning tag the attriputes which begin with the name of the attr then the assignment value 
it helps us to provide an additional info about the element and let us control the element 

every html page contains some main parts the !DOCTYPE PART AND THE HEAD PART AND THE BODY PART 
THE FIRST ONE !DOCTYPE PART we use it to let the browser know the version and the type of our file 
THE SECOND ONE THE HEAD that we define into it some data will not display in our page but it's to give data to our browser 
THE LAST ONE is the body part that we use it to define the element and everything we need to display in our page 

Here some command Example we use it in this language

`<!-- -->` this is the comment tag you can type whatever you want inside it and it will not appeare on the page

`<p>` to show normal paragraph on our page 

`<div>` we use it to group some related element in one box

`<iframe>` we use it to include another webpage in like an element in our html page 

`<meta>` we use it always in the head part and it defines some information to our browser 

let's take a look to some important attribute 

the id attribute we use it to give id for any tag and we can use one of it just on every element 

the class attribute we use it to give the tag another name that can be use to specify the element and we can use howmany class we want to the same element 

## Block level element 
        this type of elements take a full line space like `<h1> and <ul> <li> and <p>

## Inline Elements
        Some elements will always appear to continue on the same line as their neighbouring elements. These are nown as inline elements.
        Examples of inline elements are 
        <a>, <b>, <em>, and <img>

## Escape Characters
        There are some characters that are used in and reserved by HTML code. (For example, the left and right angled brackets.) like &lt; &cent; &quot;  &copy;


# New Html5 Layout Elements Contains 

Headers & Footers
`<header> <footer>`

Navigation
`<nav>`

Articles
`<article>`

Asides
`<aside>`

Sections
`<section>`

## here Example to figure out how the layout will be 
```
<!DOCTYPE html>
<html>
<head>
 <title>HTML5 Layout</title>
 <style type="text/css">
 header, section, footer, aside, nav, article, figure, figcaption { 
 display: block;} 
 body { 
 color: #666666; 
 background-color: #f9f8f6; 
 background-image: url("images/dark-wood.jpg"); 
 background-position: center; 
 font-family: Georgia, times, serif; 
 line-height: 1.4em; 
 margin: 0px;} 
 .wrapper { 
 width: 940px; 
 margin: 20px auto 20px auto; 
 border: 2px solid #000000; 
 background-color: #ffffff;} 
 header { 
 height: 160px; 
 background-image: url(images/header.jpg);} 
 h1 { 
 text-indent: -9999px; 
 width: 940px; 
 height: 130px; 
 margin: 0px;} 
 nav, footer { 
 clear: both; 
 color: #ffffff; 
 background-color: #aeaca8; 
 height: 30px;} 
 nav ul { 
 margin: 0px; 
 padding: 5px 0px 5px 30px;} 
 nav li { 
 display: inline; 
 margin-right: 40px;} 
 nav li a { 
     color: #ffffff;} 
 nav li a:hover, nav li a.current { 
 color: #000000;} 
 section.courses { 
 float: left; 
 width: 659px; 
 border-right: 1px solid #eeeeee;} 
 article { 
 clear: both; 
 overflow: auto; 
 width: 100%;} 
 hgroup { 
 margin-top:40px;} 
 figure { 
 float: left; 
 width: 290px; 
 height: 220px; 
 padding: 5px; 
 margin: 20px; 
 border: 1px solid #eeeeee;} 
 figcaption { 
 font-size: 90%; 
 text-align: left;} 
 aside { 
 width: 230px; 
 float: left; 
 padding: 0px 0px 0px 20px;} 
 aside section a { 
 display: block; 
 padding: 10px; 
 border-bottom: 1px solid #eeeeee;} 
 aside section a:hover { 
 color: #985d6a; 
 background-color: #efefef;} 
 a { 
 color: #de6581; 
 text-decoration: none;} 
 h1, h2, h3 { 
 font-weight: normal;} 
 h2 { 
     margin: 10px 0px 5px 0px; 
 padding: 0px;} 
 h3 { 
 margin: 0px 0px 10px 0px; 
 color: #de6581;} 
 aside h2 { 
 padding: 30px 0px 10px 0px; 
 color: #de6581;} 
 footer { 
 font-size: 80%; 
 padding: 7px 0px 0px 20px;}
 </style>
 <!--[if lt IE 9]>
 <script src="http://html5shiv.googlecode.com/svn/trunk/html5.js"></script>
 <![endif]-->
</head>
<body>
 <div class="wrapper">
 <header>
 <h1>Yoko's Kitchen</h1>
 <nav>
 <ul>
 <li><a href="" class="current">home</a></li>
 <li><a href="">classes</a></li>
 <li><a href="">catering</a></li>
 <li><a href="">about</a></li>
 <li><a href="">contact</a></li>
 </ul>
 </nav>
 </header>
 <section class="courses">
 <article>
 <figure>
 <img src="images/bok-choi.jpg" alt="Bok Choi" />
 <figcaption>Bok Choi</figcaption>
 </figure>
 <hgroup>
 <h2>Japanese Vegetarian</h2>
 <h3>Five week course in London</h3>
 </hgroup>

 <p>A five week introduction to traditional Japanese vegetarian meals,
 teaching you a selection of rice and noodle dishes.</p>
 </article> 
 <article>
 <figure>
 <img src="images/teriyaki.jpg" alt="Teriyaki sauce" />
 <figcaption>Teriyaki Sauce</figcaption>
 </figure>
 <hgroup>
 <h2>Sauces Masterclass</h2>
 <h3>One day workshop</h3>
 </hgroup>
 <p>An intensive one-day course looking at how to create the most delicious 
 sauces for use in a range of Japanese cookery.</p>
 </article> 
 </section>
 <aside>
 <section class="popular-recipes">
 <h2>Popular Recipes</h2>
 <a href="">Yakitori (grilled chicken)</a>
 <a href="">Tsukune (minced chicken patties)</a>
 <a href="">Okonomiyaki (savory pancakes)</a>
 <a href="">Mizutaki (chicken stew)</a>
 </section>
 <section class="contact-details">
 <h2>Contact</h2>
 <p>Yoko's Kitchen<br />
 27 Redchurch Street<br />
 Shoreditch<br />
 London E2 7DP</p>
 </section>
 </aside>
 <footer>
 &copy; 2011 Yoko's Kitchen
 </footer>
 </div><!-- .wrapper -->
</body>
</html>
```


### chapter 18 Process & Design sammary 
Firstly the chapter talk about the important of understand who your target audience
is, why they would come to your site, what information
they want to find and when they are likely to return

### Site map,
In general the sitemap is doing diagrams of the pages that will
be used to structure the site and using card sorting that help us to decide what should put information in our pages this sitemap show us like tree contains group of pages titles and it contents

### Wireframes
A wireframe is a simple sketch of the key
information that needs to go on each page of a
site. It shows the hierarchy of the information
and how much space it might require. 
wireframe like the first physiqal design to figure out what we should add and style in our pages

### Visual hierarchy 

and some design technique to edit and control our elements position in the pages to be comfortable to the users and acceptable
also read talk about Grouping and similarity and here some recap
visual hierarchy

Attention

is immediately drawn
to a picture that shows the
service this company offers
and a headline to explain it. The
size and colored background
reinforce that this is the primary
message on the page.
Should this service appeal to the

Grouping

There are several chunks of
information on this page.
At the top you can see the logo
and navigation. Under this is the
information that introduces the
company's services.
Further down are three distinct
groups showing you what the
services do, the costs involved
and some of the services' users.

Similarity

There are several examples of
similarity within this page.
The four points (at the bottom
left of the screenshot) are all
presented in a similar manner
with consistent headings and
icons.
All of the links in the body text
are in blue so it is clear what text
is clickable.

user, below they can see more
detail about what it does, how
much it costs, and who uses it.




# JAVASCRIPT 

JavaScript can be used in browsers to make websites more interactive , interesting , and user-friendly .

In computer programming, each physical thing in the world can be represented as an object. Each object can have its own properties, events and methods. The events, methods, and properties of an object all relate to each other. Using the document object, you can access and change what content users see on the page and respond to how they interact with it. All major browsers use a JavaScript interpreter to translate your instructions into instructions the computer can follow.

### The ABC of Programming
stands for:

-  What is a script and how do I create one?

-  How do computers fit in with the world around them?

-  How do I write a script for a web page? 


### How all html and css and javascript work togother 
    every one of them have own extensions and the web page work with them as a layers 
    it apply the html to display the element 
    then apply the css over it to style the element 
    then apply the javascript to make these styled elements interacts with the user and make the page more dynamic

### how to add the script to our website

    It is best to keep JavaScript code in its own JavaScript
    file. JavaScript files are text files (like HTML pages and
    CSS style sheets), but they have the . j s extension.

    The HTML <script> element is used in HTML pages
    to tell the browser to load the JavaScript file (rather like
    the <link> element can be used to load a CSS file).

    If you view the source code of the page in the browser,
    the JavaScript will not have changed the HTML,
    because the script works with the model of the web
    page that the browser has created. 

### A script
     is a series of instructions that a computer can follow one-by-one.
    Each individual instruction or step is known as a statement.
    Statements should end with a semicolon. 

### Comments
    /* Th i s script displays a greeting to the user based upon the current time.
    It is an example from JavaScript & jQuer y book */

    we can make line comment or multiline comment

### WHAT IS A VARIABLE
    the container of any data type that store and hold data with his name 
    we define it like this : Var varName = Value ;
    NOTE : we can change the variable value whenevery we want 

### Some rules to write the variable Name
    - don't start with a number
    - we can use _ or $ just from the symbols
    - we can't use any javascript keyword 
    - CASe sensitive 
    - best practise to use the name that describe his information 
    - best practise to use camel case when we need to splet the words

### Data types 
#### string
#### number
#### bool
this all data type can be hold by variables 


