Basic
CSS:

Cascading Style Sheet(CSS) is used to set the style in web pages that contain HTML elements, here we will see in how many ways we can add CSS for our HTML, there three different ways to do so one by one we will see those procedure.

External CSS:

External CSS contains a separate CSS file with a .css extension which contains only style property with the help of tag attributes.

Include external CSS file:

The external CSS file is linked to the HTML document using a link tag.

Example:

<link rel="stylesheet" type="text/css" href="/style.css" />
Internal CSS or Embedded:

CSS is embedded within the HTML file using a style HTML tag when a single HTML document must be styled uniquely.

Example:

<style type="text/css">
div { color: #444;}
</style>
Inline CSS:

It contains CSS properties in the body section specified within HTML tags using the style attribute.

Syntax:

<tag style="property: value"> </tag>
Example:

<p style="color: red"> </p>
Selectors
Selectors:

CSS selectors are used to find or selecting the HTML elements you want to style.

Universal:

Selects all elements on the pages. ‘*’ symbol is used to denote the selector as a universal selector.

Syntax:

*{property:value;}
Example:

* {
 color:green;
 text-align:center;
}
Type:

Type selector or tag name/element selector selects an HTML tag/element in your document. It selects all elements of the given type within a document.

Syntax:

p {
CSS declarations;
}
Example:

/* h1 element selected here */
h1 {
    color:green;
    text-align:center;
}
Id:

Selects an element based on the value of its unique id attribute(One id only applied to one element). An ID selector begins with a # rather than a dot character.

Syntax:

#id {css declarations; }
Example:

#colorize1 {
    color:green;
    text-align:center;
}
Class:

Selects all elements in the document that have the given class attribute. It class selector starts with a dot (.) character.

Syntax:

.class {
css declarations;
}
Example:

.colorize {
    background-color: yellow;
    font-style: italic;
    color: green;
}
Attribute:

Selects all elements that have a specified attribute. Elements grouped based on some attribute value can be styled using an attribute selector.

Syntax:

a[attribute=value] {
property: value;
}
Example:

[class] {
    text-align:center;
    Color:green;
}
div[style] {
    text-align:center;
    color:green;
    font-size:40px;
    font-weight:bold;
    margin-bottom:-20px;
}
Combinators:

Combinators are complex selectors consisting of more than one selectors having some relationship between them. These are the font-family General Sibling selector, Adjacent sibling selector, child selector, Descendant selector. General Sibling selector (~) Adjacent Sibling selector (+) Child selector (>) Descendant selector (space)

Syntax:

selector1 ~selector2 {property: value;}
selector 1+selector2{property: value;}
selector 1> selector 2 {property: value;}
selector1 selector2 {property: value;}
Example:

 div ~ p{
    color: #009900;
    font-size:32px;
    font-weight:bold;
    margin:0px;
    text-align:center;
}
Pseudo:

A Pseudo class in CSS is used to define the special state of an element to add an effect to an existing element based on its states. For ex. change of state on hover, click, focus, when a link is visited, etc.

Syntax:

selector: pseudo-class{
property: value;
}
Example:

/* hover pseudo class here */
.box:hover{
     background-color: orange;
}
Font Properties
Font Properties:

CSS font properties are used to set the font’s content of the HTML element as per requirement.

Font-family:

CSS font-family property specifies the font family to be used for the element’s text content. Different font names can be given to make a fallback system in case first in priority is unavailable.

Syntax:

font-family: family-name |generic-family |initial |inherit;
Font-style:

CSS font-style property is used to style the text content in a normal, italic, or oblique face from its font-family.

Syntax:

font-style: normal |italic |oblique |initial |inherit;
Font-variant:

CSS font-variant property is used to convert all lowercase letters into uppercase letters. The converted uppercase letters appear smaller in font-size than the original uppercase letters.

Syntax:

font-variant: normal| small caps | initial;
Font-weight:

CSS font-weight property is used to specify thickness or weight of the font in the text content of the HTML and separated color elements.

Syntax:

font-weight: normal| bold |number |initial |inherit |unset;
Font-size:

CSS font-size property is used to specify the size of the text in HTML document.

Syntax:

font-size: small |medium |large |initial |inherit;
Text Properties
Text-properties:

CSS text formatting properties are used to format and style text by setting their color, alignment, spacing, etc. as per requirement.

Text-color:

CSS text-color property is used to set the color of the text. It can be set using a comma-separatedcolor name, its hex value, or RGB value.

Syntax:

color: value;
Text-alignment:

CSS Text alignment property is used to set the horizontal alignment of the text as left, right, centered, and justified.

Syntax:

text-align: left|right|center|justify|initial|inherit;
Text-decoration:

CSS Text decoration is used to add or remove text- decorations like underline, overline, line-through or none.

Syntax:

text-decoration: decoration-type;
Text-transformation:

CSS text transformation property is used to change the case of text (Uppercase or lowercase) or capitalize text.

Syntax:

text-transform: none|capitalize|uppercase|lowercase|initial|inherit;
Text-indentation:

CSS text indentation property is used to indent the first line of text block. The size can be in px, cm, pt. size should be non-negative.

Syntax:

text-indent: length|initial|inherit;
Letter spacing:

CSS letter-spacing property is used to specify space between the characters of the text. size can be in px.

Syntax:

letter-spacing: normal|length|initial|inherit;
Line height:

CSS line spacing property is used to specify the space between the lines of the text block.

Syntax:

line-height: normal|number|length|percentage|initial|inherit;
Text-shadow:

CSS text-shadow property is used to add shadow to the text. Using this property you can specify the shadow color, horizontal size,and and vertical size for the text.

Syntax:

text-shadow: h-shadow v-shadow blur-radius color|none|initial|inherit;
Word spacing:

CSS word-spacing property is used to specify space between words of lines in the text block.

Syntax:

word-spacing: normal|length|initial|inherit;
Background properties:
Background properties:

The CSS background properties are used to design the background and define the background effects for elements.

Background-color:

CSS background-color property is used to specify the background color of an element.

Syntax:

background-color: color_name;
Example

 h2 {
    background-color:black;
}
Background-image:

CSS background-image property is used to add one or more background images to an element.

Syntax:

background-image: url(‘url’);
Example

 body {
     background-image: url("https://media.geeksforgeeks.org/wp-content/uploads/rk.png");
}
Background-repeat:

CSS background-repeat property is used to add or remove repeat the background image both horizontally and vertically.

Syntax:

background-repeat: repeat |repeat-x |repeat-y |no-repeat |initial |inherit;
Background-position:

CSS body-position property is mainly used to specify the positioning of the image in a certain way.

Syntax:

background-position: value;
Example

 body {
    background-image: url("https://media.geeksforgeeks.org/wp-content/uploads/background-position1.png");
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-position: left top;
}
Background-origin:

CSS background-origin property is used to adjust the background image of the webpage.

Syntax:

background-origin: padding-box |border-box |content-box | initial| inherit;
Background-attachment:

CSS background-attachment property is used to specify the kind of attachment of the background image with respect to its container.

Syntax:

background-attachment: scroll |fixed |local |initial |inherit;
Background-clip:

CSS background-clip property is used to define how far the background (color or image) should extend within an element.

Syntax:

background-clip: border-box| padding-box| content-box| initial |inherit;
Box Properties
Box Properties:

The CSS box model is essentially a box that wraps around every HTML element consisting of the border, padding, margin, and content.

Margin:

It sets the margin as top, left, bottom, or right by specifying length or percentage.

Syntax:

margin: value;
Example

p {
    margin: 80px 100px 50px 80px;
}
Padding:

It describes the amount of space between the border and the content of the selector.

Syntax:

padding: value;
Example p { padding: 80px 100px 50px 80px; }

Border:

It sets the element’s border width by specifying border or top, right, bottom or left border. It is also used to set the style, and color of an element’s border.

Syntax:

border: value;
Example

p {
    border: 1px solid black;
}
Width:

It sets an element’s width as a length, a percentage, or an auto.

Syntax:

width: value;
Example

div {
    width: 150px;
}
div {
    width: auto;
}
Height:

It sets an element’s height as a length, a percentage, or as auto.

Syntax:

height: value;
Example

div {
    height: 150px;
}
div {
    height: inherit;
}
Shadow properties
Shadow properties:

These shadow properties are used to add shadow to text or boxes or frames of elements to enhance the visual quality of the webpage.

Text shadow:

It is used to add shadow to text. It accepts a comma-separated list of shadow properties to be applied to the text.

Syntax:

text-shadow: h-shadow v-shadow blur-radius color| none |initial | inherit;
Box shadow:

It is used to give a shadow-like effect to the box or frames of an element. It accepts multiple comma separated effects .It is described using X and Y offsets relative to the element, blur and spread radius, and color.

Syntax:

box-shadow: h-offset v-offset blur spread color |none |inset |initial | inherit;
Gradient:
Gradient:

The CSS gradient property is used to create a smooth and progressive transition between two or more specified colors. Transition can go up/down/right/left/diagonal/radial using different color stops, angles, or percentage.

Linear Gradient:

This property is used to create smooth color transitions going up, down, left, right, and diagonally. It requires a minimum of two colors, a starting point, and the direction for the gradient effect.

Syntax:

background-image: linear-gradient(direction, color-stop1, color-stop2, …);
Example:

.gradient {
    height: 100px;
    background-image: linear-gradient(to left, yellow, blue);
}
Radial Gradient:

A radial gradient is used to obtain an elliptical shape gradient. It starts at a single point and emanates outward. The first color starts at the center position of the element and then fades to the end color towards the edge of the element at an equal pace until specified.

Syntax:

background-image: radial-gradient(shape size at position, start-color, …, last-color);
Example:

#main {
        height: 400px;
        width: 600px;
        background-color: white;
        background-image: radial-gradient(circle, green, white,blue);
}
Border Properties
Border Properties:

The CSS border properties allow you to specify how the border of the box representing an element should look. It is used to specify the color type and width of the looks border to give the element the desired look.

Border Color:

It specifies the color of the border of the box containing the element. It works only when the border-style property is defined first, it will not work alone. If this property is not set then it inherits the color of the element.

Syntax:

border-color: color-value;
Example:

div {
    border-color: red;
    height: 10px;
    width: 10px;
}
Border Style:

It sets the style or look of the border as solid, dotted, rigged, etc. It takes one to four values at a time.

Property Values:

none: No border is created and it is left plain. hidden: Just like none, it doesn’t show any border unless a background image is added, then the border-top-width will be set to 0 irrespective of the user-defined value.

dotted: A series of dots are displayed in a line as the border.

solid: A single solid and bold line is used as a border.

dashed: A series of square dashed lines are used as a border. double: Two lines placed parallel to each other act as the border.

groove: Displays a 3D grooved border, its effect depends on border-color value.

ridge: Displays a 3D ridged border, its effect depends on border-color value.

inset: displays a 3D inset border, its effect depends on border-color value.

outset: Displays a 3D outset border, its effect depends on border-color value.

Syntax:

border-style: value;
Example:

div {
    border-color: red;
    height: 10px;
    width: 10px;
    border-style: dotted;
    border-width: 2px;
}
Border Width:

It sets the width of the border of the element in length in px , cm, etc., or as thin medium, and thick.

Syntax:

border-width: length |thin |medium |thick |initial |inherit;
Example:

div {
    border-color: red;
    height: 10px;
    width: 10px;
    border-style: dotted;
    border-width: 2px;
}
Classification Properties
Classification Properties:

The CSS classification properties allow you to specify how and where an element is displayed.

Display:

Display property defines how elements are displayed in the web page.

Syntax:

display: inline |block |flex |grid |table |group |none| inherit;
Float:

It defines flow of content by determining if an element floats to the left or right, allowing text or image to wrap around it or be displayed inline.

Syntax:

float: none| left| right| initial| inherit;
Position:

It specifies the positioning method of html entity on the web page. It places an element in a fixed, static, absolute, relative or sticky position.

Syntax:

position: fixed| static| absolute |relative |sticky;
Clear:

It is used to set the sides of an element where no other floating elements are allowed.

Syntax:

clear: left |right |both | none;
Visibility:

It is used to set an element as visible or not.

Syntax:

visibility: visible |hidden | collapse |initial |inherit;
Cursor:

It is used to specify the type or shape of cursor to be displayed.

Syntax:

cursor: auto |default |pointer |crosshair |help | e-resize | all-scroll |progress |initial |inherit;
CSS Functions
CSS Functions:

CSS has a range of inbuilt functions. These are used as a value for various CSS properties. Some of the CSS functions can be nested as well. It ranges from simple color functions to mathematical, shape, color, transform, gradient, and animations functions.

attr():

CSS attr() function is an inbuilt function in CSS that retrieves the value of an attribute of the selected elements and uses it in the stylesheet.

Syntax:

attr( attr_name );
Example:

a:before {
    content: attr(href) " =>";
}
calc():

CSS calc() function takes a single mathematical expression as its parameter and performs operations based on CSS property. It can be a mix of types, such as length, number, angle and frequency.

Syntax:

calc( Expression );
Example:

div {
    position: absolute;
    left: 50px;
    width: calc(100% - 20%);
    height:calc(500px - 300px);
    background-color: green;
    padding-top:30px;
    text-align: center;
}
max():

CSS max() function returns the largest number of the given set of comma separated numbers.

Syntax:

max(value 1, value2, value3…);
Example:

.container {
    display: flex;
    justify-content: center;
    align-content: center;
    color: white;
    font-size: 30px;
    background-color: green;
    width: max(100px, 400px);
    height: max(100px, 400px);
}
url():

CSS URL() function takes a string URL as a parameter and is used to load images, fonts and content and allows you to link to a resource, such as an image, web font, a filter, etc.

Syntax:

url( <string> <url-modifier>* );
Example:

body {
    background-image: url("https://media.geeksforgeeks.org/wp-content/cdn-uploads/20190710102234/download3.png");
    text-align:center;
}
var():

CSS var() function is used to insert the value of a custom property which is the required parameter and its name must start with two dashes.

Syntax:

var( custom_property, value );
Example:

:root {
    --main-bg-color: Green; 
}
/* Use of var() function */
.div1 {
    background-color: var(--main-bg-color);
    padding:10px;
}
Media Queries
Media Queries:

The CCS Media Query is used to make the web page more responsive according to the different screens or media types. It can be used to check the width and height of the viewport or device, orientation, and resolution of the output device. It consists of a media type that can contain one or more expressions that can be either true or false. Media queries include a block of CSS only if a certain expression is true.

All: It is used for all media devices.
Print: It is used when printer is in use.
Screen: It is used for computer screens, smartphones etc.
Speech: It is used for screen readers that read the screen aloud.
Syntax:

@media not|only mediatype and (expressions) {
  CSS-Code;
}
Example:

@media screen and (min-width: 480px) {
  body {
    background-color: lightgreen;
  }
}
