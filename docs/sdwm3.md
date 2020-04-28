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

 

\- Learn how to apply different layouts in CSS

Display
=======

the CSS display property describes how an element\'s box behaves

All HTML values have a default display property.

display:block
=============

Block elements are those that start on a new line and fill their whole
container, from left to right.

 

Some block elements are **\<div\>**, **\<li\>**

display:block
=============

display.html

display:inline
==============

Inline elements do not break the flow of text in a paragraph.  Some
examples of inline-by-default elements are **\<a\>**, and **\<span\>**

display:inline
==============

display.html

display:none
============

**display:none** makes the element not to be displayed in the screen.

display:none
============

Let\'s clean up https://www.huffingtonpost.es

Default layout
==============

The default layout of web page is probably not what we want.

 

Let\'s see what\'s de default layout in HTML.

Horizontal centering
====================

One of the first things we\'ll want to do when creating the layout of a
webpage is centering the content horizontally.

 

This can be done using **margin** and **width**:

Horizontal centering
====================

but, what happens when we resize the window?

Horizontal centering
====================

**max-width** allows us to express the maximum width we want for a box,
so it resizes in case of smaller screens.

Horizontal centering
====================

Box model
=========

Remember the box model?


Box model
=========

It\'s really hard when using the box model to get the specific **width**
we want, since we need to also take **border, margin,** and **padding**
into consideration.

Box sizing
==========

Introducing box-sizing!

Position
========

we use the **position** css property to make more complex layouts.

 

There are a number of different values for it:

position:relative
=================

The relative position allows us to place the element related to where it
would be placed by default

position:fixed
==============

with the **position:fixed** attribute we can make *sticky** ***
elements.  These are elements whose position doesn\'t change even when
scrolling.

position:absolute
=================

with **position:absolute** we can place elements like with **fixed** but
relative to their *nearest positioned parent*

position
========

Float
=====

We use the **float** property to make text be able to wrap other
elements such as images

Float
=====

inline-block
============

**inline-block** is another value for display that\'s very useful when
we want to use blocks that stack besides each other!

 

Let\'s see an example!

inline-block
============

references
==========

This session was adapted from http://learnlayout.com

Workgroups
==========


Workgroups
==========

-   ~~Go to the assignments page in campus (next slide)~~
-   **one per team**, follow the link and create your respective team
-   once the team is created, everyone else follow the link and select
    your respective team

Workgroups
==========

Yesterday night campus was down so the assignment you can get it from
here:

 

https://classroom.github.com/g/N2anSgm5

 

Mind the instructions in the previous page
