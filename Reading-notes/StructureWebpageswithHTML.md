# Structure Webpages with HTML
## Here I will put my notes about the Structure Webpages with HTML topic from Read03

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

## HTML LAYOUTS
TRADITIONAL HTML
For a long time, web page authors used <div> elements to group
together related elements on the page (such as the elements that form a
header, an article, footer or sidebar). Authors used class or id attributes
to indicate the role of the <div> element in the structure of the page.
NEW HTML5 
HTML5 introduces a new set of elements that allow you to divide up the
parts of a page. The names of these elements indicate the kind of content
you will find in them. They are still subject to change, but that has not
stopped many web page authors using them already
Headers & Footers
`<header> <footer>` USING THESE TAGS
HERE EXAMPLE OF THE new layout
```
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
```

HTML5 LAYOUT 448
Example
HTML5 LAYOUT
```
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
## chapter 8 
## talk about some extra markup langueges and some commands here some exeplenaiton 

DOCTYPES tell browsers which version of HTML you
are using

You can add comments to your code between the
`<!-- and -->` markers.

The id and class attributes allow you to identify
particular elements.

The `<div> and <span>` elements allow you to group
block-level and inline elements together.

`<iframes>` cut windows into your web pages through
which other pages can be displayed.

The `<meta>` tag allows you to supply all kinds of
information about your web page.

Escape characters are used to include special
characters in your pages such as <, >, and ©.
here application on this summary 
```
<!DOCTYPE html PUBLIC
"-//W3C//DTD HTML 4.01 Transitional//EN"
"http://www.w3.org/TR/html4/loose.dtd">
<html>
<head>
 <meta name="description" content="Telephone, email
 and directions for The Art Bookshop, London, UK" />
 <title>Contact The Art Bookshop, London UK</title>
</head>
<body>
 <div id="header">
 <h1>The Art Book Shop</h1>
 <ul>
 <li><a href="index.html">home</a></li>
 <li><a href="index.html">new publications</a>
 </li>
 <li class="current-page">
 <a href="index.html">contact</a></li>
 </ul>
 </div><!-- end header -->
 <div id="content">
 <p>Charing Cross Road, London, WC2, UK</p>
 <p><span class="contact">Telephone</span>
 0207 946 0946</p>
 <p><span class="contact">Email</span>
 <a href="mailto:books@example.com">
 books@example.com</a></p>
 <iframe width="425" height="275" frameborder="0"
 scrolling="no" marginheight="0" marginwidth="0"
 src="http://maps.google.co.uk/maps?f=q&amp;
 source=s_q&amp;hl=en&amp;geocode=&amp;
 q=charing+cross+road+london&amp;output=embed">
 </iframe>
 </div><!-- end content -->
 <p>&copy; The Art Bookshop</p>
</body>
</html>
```