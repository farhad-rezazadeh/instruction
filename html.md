## HTMl

- HTML stands for Hyper Text Markup Language
- HTML is the standard markup language for creating Web pages
- HTML describes the structure of a Web page
- HTML consists of a series of elements
- HTML elements tell the browser how to display the content
- The `<!DOCTYPE html>` declaration defines that this document is an HTML5 document
- The `<html>` element is the root element of an HTML page
- The `<head>` element contains meta information about the HTML page
- The `<title>` element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
- The `<body>` element defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
- HTML tags are not case sensitive

`<tagname>`Content goes here...`</tagname>`

Some HTML elements have no content (like the `<br>` element). These elements are called empty elements. Empty elements do not have an end tag!

HTML headings are defined with the `<h1>` to `<h6>` tags.

`<p>`-paragraph

`<a>`-links==>`<a href="https://www.w3schools.com">This is a link</a>`

Attributes are used to provide additional information about HTML elements.

`<img>`-image==>`<img src="w3schools.jpg" alt="W3Schools.com" width="104" height="142">`

* Use the HTML `<img>` element to define an image
* Use the HTML `src` attribute to define the URL of the image
* Use the HTML `alt` attribute to define an alternate text for an image, if it cannot be displayed
* Use the HTML `width` and `height` attributes or the CSS `width` and `height` properties to define the size of the image
* Use the CSS `float` property to let the image float to the left or to the right

`<br>`-break

`<hr>`-horizontal line

- All HTML elements can have **attributes**
- Attributes provide **additional information** about elements
- Attributes are always specified in **the start tag**
- Attributes usually come in name/value pairs like: **name="value"**

`lang` attribute inside the `<html>` tag, to declare the language of the Web page.

The `style` attribute is used to add styles to an element, such as color, font, size, and more.

<*tagname* style="*property*:*value;*">

> font-size
>
> background-color
>
> color
>
> font-family
>
> text-align
>
> border:$SIZE solid $COLOR
>
> padding:$SIZE   ===>defines a padding (space) between the text and the border.
>
> margin:$SIZE ===>defines a margin (space) outside the border
>
> background-image

The `title` attribute defines some extra information about an element.

`<pre>`-element defines preformatted text

`<b>`-bold text

`<strong>`-important text

`<em>`-emphasized text

`<i>`-italic text

`<small>`-smaller text

`<mark>`-marked text

`<del>`-deleted text

`<ins>`-inserted text

`<sub>`-subscript text

`<sup>`-superscript text

`<blockquote>`-defines a section that is quoted from another source

```html
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature.
The world's leading conservation organization,
WWF works in 100 countries and is supported by
1.2 million members in the United States and
close to 5 million globally.
</blockquote>
```

`<q>`-define short quotation

`<abbr>`-abbreviation

`<address>`-defines the contact information 

```html
<address>
Written by John Doe.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>	
```

`<cite>` -defines the title of a creative work

`<bdo>`-to override the current text direction

```html
<bdo dir="rtl">This text will be written from right to left</bdo>
```

<!--comment in html is like this-->

HTML colors are specified with predefined color names, or with RGB, HEX, HSL, RGBA, or HSLA values.

**rgb(red,green,blue)**

**rgba(red,green,blue, alpha)**

**#rrggbb**

**hsl(hue, saturation,lightness)**

**hsla(hue,saturation, lightness, alpha)**



CSS stands for Cascading Style Sheets.

CSS can be added to HTML documents in 3 ways:

- **Inline** - by using the `style` attribute inside HTML elements

	- ```html
	  <h1 style="color:blue;">A Blue Heading</h1>
  
  	<p style="color:red;">A red paragraph.</p>
  	```

- **Internal** - by using a `<style>` element in the `<head>` section

  - ```html
    <!DOCTYPE html>
    <html>
    <head>
    <style>
    body {background-color: powderblue;}
    h1   {color: blue;}
    p    {color: red;}
    </style>
    </head>
    <body>
    
    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>
    
    </body>
    </html>
    ```


- **External** - by using a `<link>` element to link to an external CSS file

  - ```html
    <!DOCTYPE html>
    <html>
    <head>
      <link rel="stylesheet" href="styles.css">
    </head>
    <body>
    
    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>
    
    </body>
    </html>
    ```



**LINK**

* The `target` attribute specifies where to open the linked document.
  * `_self` - Default. Opens the document in the same window/tab as it was clicked
  * `_blank` - Opens the document in a new window or tab
  * `_parent` - Opens the document in the parent frame
  * `_top` - Opens the document in the full body of the window
* to use an image as a link,just put the `<img>` tag inside the `<a>` tag.
* use `mailto:` inside the `href` attribute to create a link that opens the user's email program.
* to use an html button as a link,you have to add some javascript code
* `title` attribute specifies extra information about an element

By default, a link will appear like this (in all browsers):

- An unvisited link is underlined and blue
- A visited link is underlined and purple
- An active link is underlined and red

`id` -create a bookmark.





**image map **

`<map>` tag defines an image map. An image map is an image with clickable areas. The areas are defined with one or more `<area>` tags.

```html
<img src="workplace.jpg" alt="Workplace" usemap="#workmap">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">
  <area shape="circle" coords="337,300,44" alt="Coffee" href="coffee.htm">
</map>
```



**picture**

`<picture>` element gives web developers more flexibility in specifying image resources.

>`<source>`each referring to different images through the `srcset` attribute.
>
>Each `<source>` element has a `media` attribute that defines when the image is the most suitable.

```html
<picture>
  <source media="(min-width: 650px)" srcset="img_food.jpg">
  <source media="(min-width: 465px)" srcset="img_car.jpg">
  <img src="img_girl.jpg">
</picture>
```

**Note:** Always specify an `<img>` element as the last child element of the `<picture>` element. The `<img>` element is used by browsers that do not support the `<picture>` element, or if none of the `<source>` tags matches.



**table**

`table`-define table

> `<tr>`-table row
>
> `<th>`-table header-bold and centered
>
> `<td>`-table data-regular and left-aligned
>
> `<caption>`- to add a caption to a table
>
> he `<caption>` tag must be inserted immediately after the `<table>` tag.

to add a border to a table, use the CSS `border` property:

```html
table, th, td {
  border: 1px solid black;
}
```



> `padding`-to set  pading
>
> `text-align` 
>
> `border-spacing`-to set the border spacing for a table
>
> `colspan`-to make a cell span more than one columm
>
> ```html
> <table style="width:100%">
>   <tr>
>     <th>Name</th>
>     <th colspan="2">Telephone</th>
>   </tr>
>   <tr>
>     <td>Bill Gates</td>
>     <td>55577854</td>
>     <td>55577855</td>
>   </tr>
> </table>
> ```
>
> `rowspan`-to make a cell span more than one row

adding an `id` attribute to the table can be used for define special style for one particular table.

he `<caption>` tag must be inserted immediately after the `<table>` tag.

**lists**

* unordered list

  * `<ul>`-start unordered list

  * > `list-style-type`-from style-define the style of the list item marker
    >
    > list can be nested
    >
    > also can create horizontal list

  * `<li>`-list item

* ordered list

  * `<ol>`-start ordered list

    * >`type`-define the type of the list item maker
      >
      >`start`-count from specified number
      >
      >list  can be nested

  * `<li>`-list item

* description list

  * `<dl>`-define description list
  * `<dt>`-define the term
  * `<dd>`-describe each term

  