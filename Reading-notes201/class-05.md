# Images, Color, Text

# Content Links List 

**[Images](#Images)**

**[Color](#Color)**

**[Text](#Text)**





# Images 

one image can say a thousand words and the great images it will make the difference in the website 

images should be 
- relevent 
- convey information 
- convey the right mood 
- be recognisable
- fit the color palette 

some websites provide images
- [istockphoto](www.istockphoto.com)
- [gettyimages](www.gettyimages.com)
- [veer](www.veer.com)
- [sxc](www.sxc.hu)
- [fotolia](www.fotolia.com)

### adding image to our website by using this tag `<img src="url or path then dot then the type of the image">`
We can add to this tag these attribute `alt and title and the src attribute as i mentioned before`

We can also control and edit the width, height of the image using width="" and height ="" attributes

### some software and online websites that make you able to edit and save images
 - Adobe photoshop
 - Adobe Fireworks
 - Pixelmator
 - PaintShop Pro
 - Paint.net
 - www.photoshop.com
 - www.pixlr.com
 - www.splashup.com
 - www.ipiccy.com

### There's some rules for creating images 

-   **save the image in the right format**


-   **save the image at the right size**

-   **use the correct resolution**



    JPEG  : Whenever you have many different colors in a picture you should use a JPEG

    GIF   : Use GIF or PNG format when saving images with few colors or large areas of the same color.


### Image Dimensions

    The images you use on your website should be saved at the same width and height that you want them to appear on the page.

# HTML5: Figure and Figure Caption

We can use the figure and figure caption tags to make our website more organized

        <figure>
                    <img src="images/otters.jpg" alt="Photograph of 
            two sea otters floating in water">
            <br />
            <figcaption>Sea otters hold hands when they 
            sleep so they don't drift away from each 
            other.</figcaption>
        </figure>

> Note Photographs are best saved as JPEGs; illustrations or 
logos that use flat colors are better saved as GIFs



# Color

color property allows us to specify the text color inside the element 
and background-color property we use it to change the background color of any element

We can use more than one type to write the color using the css 

- RGB VALUES `rgb(100,100,100)`
- HEX CODE `#af0000`
- COLOR NAME `red` 
- rgba `rgba(100,100,100,0.5)` to control the opacity of the color from 0 to 1
- HSL `hsl(0,0%,78%)` H this is expressed as an angle from 0 to 360 and S stand for saturation expressed as percentage and the L for lightness and expressed as percentage as well 
- HSLA `hsla(0,0%,70%,0.5)` like the hsl but the last parameter stands for Alpha to control the opacity between 0 and 1


### Contrast
 1- Low Contrast

        Text is harder to read when there is low contrast between background and foreground colors. 

 2- High Contrast

        Text is easier to read when there is higher contrast between background and foreground colors.

 3- Medium Contrast

        For long spans of text, reducing the contrast a little bit improves readability.




# Text

### Typeface Terminology 

Serif 

Sans-Serif

Monospace



## --------------------------

Weight > Light Medium Bold Black

Style > Normal Italic Oblique

Stretch > Condensed Regular Extended

> When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer.

## --------------------------------
### text properties using css

We can change the case of the letters using text-transform > uppercase , lowercase , capitalize 

We can add line to the text under line or through line by using the text-decoration property 

We can control the position of the text with using text-align property to be on the left or the center or the right or justify

also we can control the space between the letters in each word and the space between the words by using these properties letter-spacing, word-spacing
## --------------------------------
### Responding to Users

- :hover `applied when a user hovers over an element`
- :active `applied when an element is being activated by a user`
- :focus `This is applied when an element has focus`
- :link `This allows you to set styles for links that have not yet been visited. `
- :visited `This allows you to set styles for links that have been clicked on. `


## --------------------------------

### some types of Selectors 

Existence p[class] `Targets any <p> element with an attribute called class`

Equality p[class="dog"] `Targets any <p> element with an attribute called class whose value is dog`

Space p[class~="dog"] `Targets any <p> element with an attribute called class whose value is a list of space-separated words, one of which is dog`

Prefix p[attr^"d"] `Targets any <p> element with an attribute whose value begins with the letter "d"`

SubString p[attr*"do"] `Targets any <p> element with an attribute whose value contains the letters "do"`

Suffix p[attr$"g"] `Targets any <p> element with an attribute whose value ends with the letter "g"`