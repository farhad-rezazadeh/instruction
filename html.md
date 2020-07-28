## HTML

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
>
> max-width

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

```css
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


**Block and Inline Elements**

Here are the block-level elements in HTML:
```
<address><article><aside><blockquote><canvas><dd><div><dl><dt><fieldset><figcaption><figure><footer><form><h1>-<h6><header><hr><li><main><nav><noscript><ol><p><pre><section><table><tfoot><ul><video>
```

Here are the inline elements in HTML:

```
<a><abbr><acronym><b><bdo><big><br><button><cite><code><dfn><em><i><img><input><kbd><label><map><object><output><q><samp><script><select><small><span><strong><sub><sup><textarea><time><tt><var>
```

`<div>`-is often used as a container for other HTML elements.

`<span>`-is an inline container used to mark up a part of a text, or a part of a document.

`class`-attribute is used to specify a class for an HTML element.

`id`-attribute is used to specify a unique id for an HTML element.

`<iframe>`-specifies an inline frame. an inline frame is used to embed another document within the current HTML document.

>```html
><iframe src="url" title="description">
>```
>```html
><iframe src="demo_iframe.htm" height="200" width="300" title="Iframe Example"></iframe>
>```
>
>```html
><iframe src="demo_iframe.htm" style="height:200px;width:300px;" title="Iframe Example"></iframe>
>```
>
>```html
><iframe src="demo_iframe.htm" style="border:none;" title="IframeExample"></iframe>
>```
>



**Iframe - Target for a Link**

```html
<iframe src="demo_iframe.htm" name="iframe_a" title="Iframe Example"></iframe>

<p><a href="https://www.w3schools.com" target="iframe_a">W3Schools.com</a></p>
```



**HTML Javascript**

`<script>` tag is used to define a client-side script(JavaScript)

`<nonscript>`-tag defines an alternate content to be displayed to users that have disabled script in their borwser.

<hr>

**`<meta>`**-is typically used to specify the character set,page description,keywords,author of the document,and viewport settings.

**Define the character set used:**

```html
<meta charset="UTF-8"
```

**Define the character set used:**

```html
<meta name="keywords" content="HTML, CSS,JavaScript">
```

**Define a description of your web page:**

```html
<meta name="description" content="Free Web tutorials">
```

**Define the author of a page:**

```html
<meta name="author" content="John Doe">
```

**Refresh document every 30 seconds:**

```html
<meta http-equiv="refresh" content="30">
```

**Setting the viewport to make your website look good on all devices:**

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

>The viewport is the user's visible area of a web page. It varies with the device - it will be smaller on a mobile phone than on a computer screen.
>
>```html
><meta name="viewport" content="width=device-width, initial-scale=1.0">
>```



`<base>`-specifies the base URL and/or target for all relatvie URLs in a page.



**HTML Layout Elements**

Semantic elements = elements with a meaning.

- `<header>` - Defines a header for a document or a section
- `<nav>` - Defines a set of navigation links
- `<section>` - Defines a section in a document
- `<article>` - Defines an independent, self-contained content
- `<aside>` - Defines content aside from the content (like a sidebar)
- `<footer>` - Defines a footer for a document or a section
- `<details>` - Defines additional details that the user can open and close on demand
- `<summary>` - Defines a heading for the `<details>` element
- `<figure>`-specifies self-contained content,like illustrations,diagrams,photos,code listings,etc
- `<figcaption>`-define a caption for a `<figure>` element.
- `<time>`-define specific time
- `<main>` -specifies the main content of a document.
- `<details>`-define additional details that the user can view or hide.
- `<summary>`-defines a visible heading for `<details>` element.

**HTML Computer Code Elements**

`<kdb>`-keyboard input

`<samp>`-define sample output from a computer program

`<code>`-define a piece of computer code.

`<var>`-define a variable in programming or in a mathematical experssion.

**URL**

> scheme://prefix.domain:port/path/filename

- **scheme** - defines the **type** of Internet service (most common is **http or https**)
- **prefix** - defines a domain **prefix** (default for http is **www**)
- **domain** - defines the Internet **domain name** (like w3schools.com)
- **port** - defines the **port number** at the host (default for http is **80**)
- **path** - defines a **path** at the server (If omitted: the root directory of the site)
- **filename** - defines the name of a document or resource

**HTML forms**

`<form>`-create an HTML form for user input

> `action`-defines the action to be performed when the form submitted
>
> `target`-if the submit  if the submitted result will open in a new browser tab, a frame, or in the current window.
>
> `method` attribute specifies the HTTP method (**GET** or **POST**) to be used when submitting the form data.
>
> 

`<input>`-can be displayed in many ways, depending on the `type` attribute.

>"text"-Displays a single-line text input field
>
>"radio"-Displays a radio button
>
>"submit"-Displays a submit button

**`<input type="text">`**

defines a single-line input field for **text input**.

`<label>`-defines a label for many form elements.

```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname">
</form>
```

**`<input type="radio">`**

Radio buttons let a user select ONE of a limited number of choices.

```html
<form>
  <input type="radio" id="male" name="gender" value="male">
  <label for="male">Male</label><br>
  <input type="radio" id="female" name="gender" value="female">
  <label for="female">Female</label><br>
  <input type="radio" id="other" name="gender" value="other">
  <label for="other">Other</label>
</form>
```

**`<input type="submit">`**

defines a button for **submitting** the form data to a **form-handler**.

```html
<form>
  <label for="fname">First name:</label><br>
  <input type="text" id="fname" name="fname" value="John"><br>
  <label for="lname">Last name:</label><br>
  <input type="text" id="lname" name="lname" value="Doe"><br><br>
  <input type="submit" value="Submit">
</form>
```

The `<form>` element can contain one or more of the following form elements:
```html
<label>
<input>
<select>
<textarea>
<button>
<fieldset>
<legend>
<datalist>
<output>
<option>
<optgroup>
```

**`<select>`**-define a drop-down list

```html
<label for="cars">Choose a car:</label>
<select id="cars" name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>

```

**`<option>`**-define an option that can be selected.

**`<size>`**-specify the number of visible values.

```html
<label for="cars">Choose a car:</label>
<select id="cars" name="cars" size="3">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select>
```

**`multiple`**-allow user to select multiple more than one value.

**`<optgroup>`**-to group related options in a drop-down list

```html
<form action="/action_page.php">
  <label for="cars">Choose a car:</label>
  <select name="cars" id="cars">
    <optgroup label="Swedish Cars">
      <option value="volvo">Volvo</option>
      <option value="saab">Saab</option>
    </optgroup>
    <optgroup label="German Cars">
      <option value="mercedes">Mercedes</option>
      <option value="audi">Audi</option>
    </optgroup>
  </select>
  <br><br>
  <input type="submit" value="Submit">
</form>
```



**`<textarea>`**-define multiple line input field.

```html
<textarea name="massage" rows="10" cols="30">
the cat was playing in the garden.
</textarea>
```

**`<button>`**-defines a clickable button.

```html
<button type="button" onclick="alert('Hello World!')">Click Me!</button>
Try it Yourself »
```

**`<fieldset>`**-used to group related data in a form.

**`<legend>`**-defines a caption for the `<fieldset>` element.

**`<datalist>`**-specifies a list of pre-defind options for an `<input>` element

The list attribute of the `<input>` element, must refer to the id attribute of the `<datalist>` element.

```html
<form>
	<input list="browsers">
	<datalist id="browsers">
		<option value="internet explore">
		<option value="firefox">
		<option value="chrome">
		<opiton value="safari">
	</datalist>
</form>
```

**`<output>`**-represents the result of calculation.

```html
<form action="/action_page.php"
  oninput="x.value=parseInt(a.value)+parseInt(b.value)">
  0
  <input type="range"  id="a" name="a" value="50">
  100 +
  <input type="number" id="b" name="b" value="50">
  =
  <output name="x" for="a b"></output>
  <br><br>
  <input type="submit">
</form>
```



**`<input type="password">`**-defines a password field

**`<input type="reset">`**-defines a reset button that will reset all form value to their default

**`<input type="checkbox">`**-defines a checkbox

**`<input type="color">`**-used to input that should contain a color

**`<input type="date">`**-used for input fields that should contain a date.

> **`min`** & **`max`** attributes to add restrictions to dates

**`<input type="datetime-local">`**-specifies a date and time input field, with no time zone.

**`<input type="email">`**-is used for input fields that should contain an e-mail address.

**`<input type="file">`**-define a file-select and "browse" button for file uploads.

**`<input type="month">`**-allows the user to select a month and year.

**`<input type="number">`**-define a numeric input field.

> | Attribute | Description                                                  |
> | :-------- | :----------------------------------------------------------- |
> | checked   | Specifies that an input field should be pre-selected when the page loads (for type="checkbox" or type="radio") |
> | disabled  | Specifies that an input field should be disabled             |
> | max       | Specifies the maximum value for an input field               |
> | maxlength | Specifies the maximum number of character for an input field |
> | min       | Specifies the minimum value for an input field               |
> | pattern   | Specifies a regular expression to check the input value against |
> | readonly  | Specifies that an input field is read only (cannot be changed) |
> | required  | Specifies that an input field is required (must be filled out) |
> | size      | Specifies the width (in characters) of an input field        |
> | step      | Specifies the legal number intervals for an input field      |
> | value     | Specifies the default value for an input field               |

**`<input type="range">`**-define a control for entering a number whose exact value is not important

>`min`
>
>`max` 
>
>`step`

**`<input type="search">`**-is used for search fields

**`<input type="tel">`**-is used for input fields that should contain a telephone number.

**`<input type="time">`**-select time.

**`<input type="url">`**-input field that should contain a URL address.

**`<input type="week">`**-allows user to select a week and year.

