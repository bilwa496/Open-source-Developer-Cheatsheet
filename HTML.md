HTML
HTML stands for Hyper Text Markup Language. It is a language used to make websites. A HTML file is made of 2 things.
1) Elements
2) Their Attributes
HTML Anatomy
The very basic structure of a HTML document consists of a html,head, body elements. The (!DOCTYPE html) is added at the start of every document. It is a document type declaration which is a set of guidelines and regulations that must be attached to a certain online document(html,xml etc).
<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title></title>
  </head>
  <body>
    
  </body>
</html>
Elements
There are many types of HTML elements. Some of them are
HTML HEADINGS
<h1> Heading 1 </h1>
<h2> Heading 2 </h2>
<h3> Heading 3 </h3>
<h4> Heading 4 </h4>
<h5> Heading 5 </h5>
<h6> Heading 6 </h6>
which looks like this:


PARAGRAPH TAG
It is one of the basic tags of HTML. It is used to define certain text as paragraph.
<p>This is a part of a paragraph </p>
OUTPUT: This is a part of a paragraph.


To italisize text in html we can use the italic or emphasise tags.Italic tag italisises the text inside it ,that is, it styles the text to make it slanted. But the text inside the em or emphasise tag is stresses and emphasised.
This is <i> italic </i>
This is <em> emphasised </em>
This is italic
This is * emphasised*

To make text bold 2 tags can be used. Bold or strong.
This is <b> bold </b>
This is <strong> strong </strong>
OUTPUT:
This is bold
This is strong

They can be together used in paragraph tag as follows.
  <p> I am <em> writing </em> a <strong>HTML</strong> cheatsheet.    
which looks like this:
I am writing a HTML cheatsheet.

HTML LISTS
There are 2 types of lists in HTML.
---> Ordered list(ol)
An ordered list is something that renders a list which is numbered. The various items inside a list are specified using (li) tag.
<ol>
 <li>This</li>
 <li>is</li>
 <li>an</li>
 <li>ordered list</li>
</ol>
OUTPUT:

This
is
an
ordered list


Attributes
1. Type: Sets the numbering type
<ol type="a">
<li>a for lowercase letters
</ol>
<ol type="A">
<li>A for uppercase letters
</ol>
<ol type="i">
<li>i for lowercase Roman numerals
</ol>
<ol type="I">
<li>I for uppercase Roman numerals
</ol>
<ol type="I">
<li>1 for numbers (default)
</ol>
OUTPUT:


Start: Used to change the starting numbering value. For example, to start a ordered list from 6 we can specify start ="6".
<ol start ="6" type="a">
<li>This</li>
<li>is</li>
<li>an</li>
<li>ordered list</li>
</ol>
OUTPUT:

This
is
an
ordered list

---> Unordered list(ul)
An unordered list is something that renders a list which is bulleted. The various items inside a list are specified using (li) tag.
<ul>
 <li>This</li>
 <li>is</li>
 <li>an</li>
 <li>unordered list</li>
</ul>
OUTPUT:

This
is
an
unordered list

Attributes

1. Type: Sets the type of bullets
<ul type="circle">
<li>circle
</ul>
<ul type="disc">
<li>disc
</ul>
<ul type="square">
<li>square
</ul>
OUTPUT:

circle
disc
square
HTML IMAGE ELEMENTS
Images can be added to HTML using the (img) tag. But the image tag is not enough, we should also specify the source(src attribute) of the image to display a particular image.The source can be either local or on the web.
<img src="image.png">
The various attributes of image are:

src- Specifies the path to the image
alt-Specifies an alternate text for the image, if the image for some reason cannot be displayed
width- Specifies the width of the image
height- Specifies the height of the image
HTML LINKS ANCHOR TAGS
The HTML tag also known as the HTML anchor tag is used to specify a hyperlink to link one page to another. The hyperlink can be created to another web page or a file, a location, or a URL. To link to destination page or URL, the “href” attribute is used with the HTML anchor tag.
<p> This is linked to 
<a href="https://github.com"> Github </a>
</p>
OUTPUT:

This is linked to Github


To apply the styles styled using CSS in the file styles.css we can use links.
<link rel="stylesheet" href="styles.css">
HTML TABLES
A HTML table contains rows and columns.To declare a table we use the (table) tag. To add rows to the table (tr)- table row tag can be used. To specify table hedings (th) tag can be used.To add data inside a table cell (td) tag is used. Columns can be created using both (th) and (td) tags. The contents inside (th) tag are bold.
<table>
<tr>
 <th>Column-1</td>
 <th>Column-2</td>
 <th>Column-3</td>
</tr>
<tr>
 <td>Text-1</td>
 <td>Text-2</td>
 <td>Text-3</td>
</tr>
<tr>
 <td>Content-1</td>
 <td>Content-2</td>
 <td>Coontent-3</td>
</tr>
</table>
OUTPUT:

Column-1	Column-2	Column-3
Text-1	Text-2	Text-3
Content-1	Content-2	Coontent-3
HTML FORMS
An HTML form is used to collect user input. The user input is most often sent to a server for processing.The HTML (form) element is used to create an HTML form for user input.The (form) element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.The HTML (input) element is the most used form element.
An (input) element can be displayed in many ways, depending on the type attribute.

Here are some examples:

Type	Description
Text	Displays a single-line text input field
Radio	Displays a radio button (for selecting one of many choices)
Checkbox	Displays a checkbox
Submit	Displays a submit button
Button	Displays a clickablebutton
The (label) tag defines a label for many form elements.The for attribute of the (label) tag should be equal to the id attribute of the element to bind them together.

<label for="name">Your Name:</label>
<input type="text" id="name"><br>
<label for="yes">Yes </label>
<input type="Radio" id="yes"><br>
<label for="no">No</label>
<input type="checkbox" id="no"><br>
<input type="submit">
OUTPUT:


For further information regarding HTML elements and their attributes,refer to:
https://www.w3schools.com/html
https://developer.mozilla.org/en-US/docs/Web/HTML
