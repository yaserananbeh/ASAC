# Color
## Here I will put my notes about Color topic from Read 06b



The **Color** property allows you to specify the color of the text inside an element , and you can specify any color using css in three ways :
- By color name 
        color: DarkCyan;
- By Hex code 
        color: #ee3e80;
- By RGB value
        color: rgb(100,100,90);


**Background-color** 

CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.

**Understanding Color**
Every color on a computer screen is created by mixing amounts of red,
green, and blue. To find the color you want, you can use a color picker.

**RGB Values**
Values for red, green, and blue
are expressed as numbers
between 0 and 255. 

**Hex Codes**
Hex values represent values
for red, green, and blue in
hexadecimal code

**Color Names**
Colors are represented by
predefined names. However,
they are very limited in number.

**Hue**
Hue is near to the colloquial idea
of color. Technically speaking
however, a color can also have
saturation and brightness as
well as hue.

**Saturation**
Saturation refers to the amount
of gray in a color. At maximum
saturation, there would be no
gray in the color. At minimum
saturation, the color would be
mostly gray

**Brightness**
Brightness (or "value") refers
to how much black is in a color.
At maximum brightness, there
would be no black in the color.
At minimum brightness, the
color would be very dark.

## Note , it is important to ensure that there is enough contrast for the text to be legible.
    Low contrast the text harder to read and there's low contrast between the background and the text
    high contrast the text will be easy to read but the cotrast between the background color and the text is high
    medium contrast this type we reduce the contrast a little bit but we improve the readability


### In Css3 become able to control the opacity of the element this opacity we put it in the last parameter in     rgba(R,G,B,Opacity) and it will be from 0.0 to 0.1

## Also in css3 we become able to use the HSL & HSLA
**hue**
This is expressed as an angle
(between 0 and 360 degrees).

**saturation**
This is expressed as a
percentage.

**lightness**
This is expressed as a
percentage with 0% being white,
50% being normal, and 100%
being black

**alpha**
This is expressed as a
number between 0 and 1.0.
For example, 0.5 represents
50% transparency, and 0.75
represents 75% transparency


## **HERE I WILL PROVIDE BIG EXAMPLE TO USE COLOR IN OUR PAGE**
```
<!DOCTYPE html>
<html>
<head>
 <title>Color</title>
 <style type="text/css">
 body {
 background-color: silver;
 color: white;
 padding: 20px;
 font-family: Arial, Verdana, sans-serif;}
 h1 {
 background-color: #ffffff;
 background-color: hsla(0,100%,100%,0.5);
 color: #64645A;
 padding: inherit;}
 p {
 padding: 5px;
 margin: 0px;}
 p.zero {
 background-color: rgb(238,62,128);}
 p.one {
 background-color: rgb(244,90,139);}
 p.two {
 background-color: rgb(243,106,152);}
 p.three {
 background-color: rgb(244,123,166);}
 p.four {
 background-color: rgb(245,140,178);}
 p.five {
 background-color: rgb(246,159,192);}
 p.six {
 background-color: rgb(245,176,204);}
 p.seven {
 background-color: rgb(0,187,136);}
 p.eight {
 background-color: rgb(140,202,242);}
 p.nine {
 background-color: rgb(114,193,240);}
 p.ten {
 background-color: rgb(84,182,237);}
 p.eleven {
 background-color: rgb(48,170,233);}
 p.twelve {
 background-color: rgb(0,160,230);}
 p.thirteen {
 background-color: rgb(0,149,226);}
 p.fourteen {
 background-color: rgb(0,136,221);}
 </style>
</head>
<body>
 <h1>pH Scale</h1>
 <p class="fourteen">14.0 VERY ALKALINE</p>
 <p class="thirteen">13.0</p>
 <p class="twelve">12.0</p>
 <p class="eleven">11.0</p>
 <p class="ten">10.0</p>
 <p class="nine">9.0</p>
 <p class="eight">8.0</p>
 <p class="seven">7.0 NEUTRAL</p>
 <p class="six">6.0</p>
 <p class="five">5.0</p>
 <p class="four">4.0</p>
 <p class="three">3.0</p>
 <p class="two">2.0</p>
 <p class="one">1.0</p>
 <p class="zero">0.0 VERY ACID</p>
</body>
</html>
```