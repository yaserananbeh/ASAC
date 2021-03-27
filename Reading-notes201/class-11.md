# Audio, Video, Images

## Images

- We can control the size of any image in the website by using the width and the height css attributes
- usually we control the size of images in this way instead of use the image size because the html and css load before the images and it's good to tell the browser how much space we need to the images 
- aligning the images we can set the align by add float attribute to the img selector to display on the left or the right
- images by default it's inline block if we need to center the image we have to make them display as a block by change this attribute to display:block 
- there's two way to center the images in the page the first one give the container of the image porperty text-align center or give to the image it self margin auto from left and right after we change the image to be block element 
- we can give the image to any element on the page to be as a background to it by using this attribute background-image: url('the path or the url'); but take this note we said before the image the last thing load in the page and make the site take more time to load 
- background repeat this attribute we use it to control the times that we need to repeat the image in the background and these the values to this attribute (no-repeat, repeat-x, repeat-y and repeat(the default))
- background-attachment (fixed or sroll ) to control the image if we need to stay in the same position or we need it to move with scrolling 
- background-position this attribute make us able to control the position of the background to be (left top,left center , left bottom, center left , center center , center bottom , right top , right center , right bottom )
- we can type shorthand to the background properties `background: #ffffff url("images/tulip.gif")  no-repeat top right;` 


## Search Engine Optimization
- SEO stands for search engine optimaization and this mean we should follow some rules to enhance the findability of our website 
- On page SEO (there's seven places in your website the engine will take their text to be conseder about the page topic )(the page title, the url , the headings in the page , Text, link text , Image alt text and the last place is the page desciption)

- six steps that will help you identify the right keywords and phrases for your site ( brainstorm, organize , research , compare , refine And map )
- we can use Google Analytics service to analyze how the visitors found the website, what they were looking at and at what point they are leaving.
- we also can to show how many people are coming to the website , and what the visitors looking at and where the visitors coming from 
- in order to put our websit on the web we will need a domain name and a web hosting 
- the domain name is the web address to the website 
- Web hosting this service make us able to upload our website files on a web server which it consistantly connect to the internet to send the website pages to the users who requested it 
- to upload the files to the webserver we need to transfer our files to the hosting server using the FTP which is the protocol that responsible about send the files on the internet 


## HTML5 video and audio

- The `<video>` and `<audio>` elements allow us to embed video and audio into web pages.

```
<video controls>
  <source src="rabbit320.mp4" type="video/mp4">
  <source src="rabbit320.webm" type="video/webm">
  <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
</video>
```