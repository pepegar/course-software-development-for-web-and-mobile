---
title: Software Development for Web and Mobile
author: Pepe García
email: jgarciah@faculty.ie.edu
date: 2020-04-20
lang: en
---

Software Development for Web and Mobile
=======================================


Grading system
==============

  Criteria              Score %
  --------------------- ---------
  Final Exam            20 %
  Individual Work       40 %
  Workgroups            20 %
  Class Participation   20 %

Course structure
================

The structure of the course will remain the same, with lectures, lab
sessions, and a final exam.

 

There will be individual assignments, and group assignments.

Changes in assignments
======================

Code assignments are a pain in the back, so we\'re changing the approach
and relying on Github for everything.

 

For you the process will be similar to the one we\'ve been following for
the last assignments.

Syllabus
========

Sessions 1 & 2 (today)
======================

-   Remember how the Internet works
-   Recap on HTTP servers and HTTP clients
-   Web browsers
-   Introduce web technologies: HTML & CSS
-   Start learning HTML

Sessions 3 & 4
==============

-   More HTML!
-   Styling web pages: CSS
-   CSS: How does it work?
-   different ways to include it in a web page

Sessions 5 & 6
==============

-   CSS in more depth
-   CSS precedence
-   Lab session!

Sessions 7 & 8
==============

-   Dinamic HTML
-   Javascript
-   JS libraries

Sessions 9 & 10
===============

-   Python for the backend
-   Web servers
-   Handling data from the frontend

Session 11
==========

-   More backend

Session 12
==========

-   lab session. Backend + frontend

Sessions 13, 14 & 15
====================

-   Back - front communication.
-   AJAX

Session 16
==========

-   Lab: Back - front communication.

Session 17
==========

-   Final exam

HTTP Recap
==========

HTTP
====

What\'s HTTP?

A protocol

Based on clients and servers

Clients sends requests to servers. Servers answer with responses

HTTP Methods
============

  method       **intention**
  ------------ ----------------------
  **GET**      access to a resource
  **POST**     update a resource
  **PUT**      create a resource
  **DELETE**   delete a resource

HTTP Server
===========

Let\'s create a server that receives a name and answers saying hello,
name

HTTP Client
===========

Let\'s create a function that uses **requests** to get a salutation from
the server

HTML
====

**HTML** stands for **Hypertext Markup Language**.  It\'s a language
that describes how the information\
should be presented in webpages

CSS
===

**CSS** stands for **Cascading Style Sheets**.  It\'s the language to
describe presentation of webpages (colors, fonts, sizes, etc).

Web browsers
============

What are web browsers?

HTTP clients

With a rendering engine

Lifecycle of a web request
==========================

Browser sends HTTP request to server

Server responds with the HTML

Browser renders the HTML

Browser gets the CSS and applies it to the page

HTML example
============

Let\'s see how HTML and CSS works in a well known web application:
Github

Other web browsers
==================

Not all browsers are equal, lets use lynx to browse the web :)

Code editors
============

So far we\'ve only used spyder for code editing, but it only works on
python.

 

Now we\'ll need other code editor:

Install VScode
==============

Install Visual Studio code from https://code.visualstudio.com/

 

(You may already have it from when you installed anaconda)

HTML
====

HTML documents are defined by tags, which look as follows:

``` {.xml}
<tag>content</tag>
```

HTML
====

Let\'s dissect that piece of code:

**\<tag\>** is the opening tag

**\</tag\>** is the closing tag

**content** is the\... content of that tag. (it may contain other tags
as well)

HTML
====

Let\'s see a real world example

``` {.xml}
<p>this is a paragraph</p>
```

the \<p\> tag is used to represent paragraphs!

HTML structure
==============

In HTML, all the visible structure of the document must go inside the
**\<body\>** tag

``` {.xml}
<body>
  <p>the 'p' tag represents a paragraph</p>
</body>
```

HTML structure
==============

On the other hand, all the HTML tags that are not meant to be rendered
go inside the **\<head\>** tag.\
\
For example, the title tag is one of these tags:

``` {.xml}
<head>
  <title>this is the title</title>
</head>
<body>
  <p>the 'p' tag represents a paragraph</p>
</body>
```

HTML structure
==============

Finally, for an HTML document to be well formed, it needs to be wrapped
in the HTML tag

``` {.xml}
<html>
  <head>
    <title>this is the title</title>
  </head>
  <body>
    <p>the 'p' tag represents a paragraph</p>
  </body>
</html>
```

HTML structure
==============

Let\'s create our first web page!

Some HTML tags
==============

Now let\'s see some HTML tags

Paragraphs
==========

text paragraphs in HTML are represented with the **\<p\>** tag

``` {.xml}
<p>
this is the first paragraph of my text.  As you can see it
also contains <strong>other tags</strong>
</p>
<p>
In the second paragraph, I wanted to write this other thing
but I'm running out of ideas for what to write
</p>
<p>
In the last paragraph of my text I want to <strong>finish</strong>
it
</p>
```

Paragraphs
==========

text paragraphs in HTML are represented with the **\<p\>** tag

``` {.xml}
<p>
this is the first paragraph of my text.  As you can see it
also contains <strong>other tags</strong>
</p>
<p>
In the second paragraph, I wanted to write this other thing
but I'm running out of ideas for what to write
</p>
<p>
In the last paragraph of my text I want to <strong>finish</strong>
it
</p>
```

Headings
========

Headings are used in html in the same way a word doc, or in a newspaper,
to capture reader\'s attention.


What\'s the most important heading in the image? and the second one?

Headings
========

HTML provides us with 6 different tags to represent 6 different levels
of headings: **\<h1\>**, **\<h2\>**, **\<h3\>**, **\<h4\>**, **\<h5\>**,
and **\<h6\>**.

``` {.xml}
<h1>this is the h1</h1>
<h2>this is the h2</h2>
<h3>this is the h3</h3>
<h4>this is the h4</h4>
<h5>this is the h5</h5>
<h6>this is the h6</h6>
```

Headings
========

Here\'s an example of the headings of these slides:

``` {.xml}
- Preamble
  - Course structure
  - Changes in assignments and exercises
  - Go over syllabus together
```

Headings
========

We could represent the previous headings in HTML as follows:

``` {.xml}
<html>
  <head></head>
  <body>
    <h1>Preamble</h1>
    <h2>course structure</h2>
    <h2>Changes in assignments and exercises</h2>
    <h2>Go over the syllabus together</h2>
  </body>
</html>
```

Hyperlinks
==========

Hyperlinks are the most vital part of HTML.  They allow us to go to
other documents when clicking them.


Hyperlinks
==========

We create links in HTML using the **\<a\>** tag.

``` {.xml}
<a>this is a link, but doesn't have an address to go to...</a>
```

In order to give an address to the link, we need to use the **href
attribute**:

``` {.xml}
<a href="https://google.com">this takes you to Google!</a>
```

Homework
========

Homework
========

Create the HTML for what it could be your Wikipedia entry.

 

\- different parts of your life

\- links to your presence in the web

Resources
=========

Free course to learn HTML: https://www.codecademy.com/courses/learn-html

Mozilla development network docs:

https://developer.mozilla.org/en-US/docs/Web/HTML
