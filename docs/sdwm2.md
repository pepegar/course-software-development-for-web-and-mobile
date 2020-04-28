---
title: Software Development for Web and Mobile
author: Pepe García
email: jgarciah@faculty.ie.edu
date: 2020-04-20
lang: en
---

Software Development for Web and Mobile
=======================================


Plan for today
==============

Today we will:

\- Learn some other HTML tags

\- Learn how CSS selectors work

\- learn some CSS rules

\- Learn about CSS box model

 

The new organization
====================

Do not create repositories there directly, create them in your own
profile ;)

HTML tables
===========

Tables are created with the \<table\> element

    <table>
    </table>

HTML tables
===========

Content in HTML tables is added by creating rows and cells.

 

Rows are created with the \<tr\> element:

``` {.gams}
<table>
  <tr></tr>
  <tr></tr>
  <tr></tr>
</table>
```

This table will have three rows

HTML tables
===========

Finally, cells in tables re created with the \<td\> element

``` {.gams}
<table>
  <tr>
    <td>row 1, cell 1</td>
    <td>row 1, cell 2</td>
  </tr>
  <tr>
    <td>row 2, cell 1</td>
    <td>row 2, cell 2</td>
  </tr>
</table> 
```

HTML images
===========

We add images to an HTML document with the HTML tag:

``` {.gams}
<img src="path to the image"/>
```

HTML images
===========

So, what can we put in the src **attibute**?

 

\- an **absolute** path

\- a **relative** path

\- a full **url** pointing to the image in the internet

HTML images
===========

Other important **attribute** of the **img** tab is the **alt
attribute:**

``` {.gams}
<img src="dog.jpg" alt="a very beautiful dog"/>
```

the **alt** attribute is used when the browser cannot display the
element, such as in browsers for people with visual impairments

HTML images
===========

https://github.com/mcsbt-2019-web-and-mobile/session2-exercises

**Let\'s do exercise 1!**

CSS
===

\- What is CSS\
- how to add CSS to a webpage\
- cascading, precendence

CSS
===

CSS is a language to give style to webpages.

CSS
===

``` {.gams}
p {
  color: 000;
  blackground: orange;
  padding: 15px;
}
```

Adding CSS to a webpage
=======================

There are several ways to add css to a webpage:

\- using the **style=\"\"** attribute

\- using the **\<style\>** html tag

\- loading the CSS from an external resource

Adding CSS to a webpage
=======================

one can use the **style** attribute to add style to an HTML element
directly

``` {.gams}
<p style="border:2px;">
this paragraph will have a two pixels border
</p>
```

Adding CSS to a webpage
=======================

Let\'s add a border to all dog images in the table!

Adding CSS to a webpage
=======================

Using the **\<style\>** tag:

``` {.gams}
<style>
  p {
    border: 2px;
  }
</style>
```

Adding CSS to a webpage
=======================

Let\'s add a border to all dog images in the table!

Adding CSS to a webpage
=======================

Loading an external CSS file:

``` {.gams}
<link rel="sylesheet" href="file.css">
```

Adding CSS to a webpage
=======================

Let\'s add a border to all dog images in the table!

CSS rules
=========

CSS rules are formed by keys and values, separated by a colon, and
finished by a semicolon:

``` {.gams}
key: value;
```

CSS rules. Styling text
=======================

How can we give style to text

``` {.gams}
color: #000;
font-family: arial;
font-size: 22px;
font-style: italic;
font-weight: bold;
text-decoration: underline;
text-align: justify;
```

CSS rules. Styling text
=======================

How can we give style to text

The box model
=============

All tags in HTML will behave as boxes.  These boxes have some common
properties that we need to be aware of.

The box model
=============


The box model
=============

\- **width** and **height** apply to the content of the box

\- The **padding** is the distance from the content to the border

\- The **border** sits between the margin and padding

\- The **margin** is the distance from the border to the other elements

The box model
=============

``` {.gams}
background: #000;
width: 100px;
padding: 20px;
margin: 20px;
border: 5px solid orange;
```

some CSS rules that we can apply to boxes:

CSS rules
=========

https://github.com/mcsbt-2019-web-and-mobile/session2-exercises

**Let\'s do exercise 2!**

CSS selectors
=============

Selectors define the elements to which a CSS rule apply.

 

For example, if we want to apply a CSS rule to all images, we can use
the **img** selector.

element selectors
=================

In element selectors we use the element name to select it:

``` {.gams}
h1 {
  color: #EEE;
}

p {
  text-align: justify; 
}
```

class selectors
===============

We can give a class to HTML elements so we can refer to it from CSS
later on:

``` {.gams}
<p class="red-text">this text will be red</p>
```

``` {.gams}
.red-text {
  color: red;
}
```

**HTML:**

**CSS:**

class selectors
===============

classes can be used to create reusable sets of styles

id selectors
============

We use the id attribute to give a unique identifier to a tag in the
document.  We can refer to it from the CSS later:

``` {.gams}
<h1 id="title">title</h1>
```

``` {.gams}
#title {
  font-size: 50px;
  color: #000;
}
```

**HTML:**

**CSS:**

CSS dinner!
===========

https://flukeout.github.io/

HTML divs
=========

the **div** tag is used in HTML to structure the content of an HTML web
page.

 

We normally use them together with **classes** and **ids** for a better
styling.

HTML divs
=========

``` {.gams}
<div id="tweetstream">
  <div class="tweets">
    <div class="tweet">
      <img src="profile.jpg">
      <p>this is the #content of the tweet</p>
    </div>
    <div class="tweet">
      <img src="profile.jpg">
      <p>this is the #content of the tweet</p>
    </div>
  </div>
</div>
```

Exercise 3
==========

Exercises
=========

Exercises
=========

Add styles to your Wikipedia page!

Exercises
=========

Investigate about CSS **display** property.

 

Create a web page simulating a blog, in which you have a **header**,
content with **articles**, a **sidebar**, and a **footer**

Exercises
=========

Investigate about grid layouts with CSS.

 

Create a proof of concept page simulating **pinterest**.
