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

 

\- Learn how to communicate with the backend

\- Review last day exercises

\- Do some exercises in class

Fetch
=====

**fetch** is the way of calling HTTP services from Javascript.

    fetch("url"); //done!

Fetch
=====

We can customize our request using the second parameter:

    fetch(
        "url",
        {
            method: "POST",
            headers: {},
            body: "this is the body"
        }
    );

Fetch
=====

but, how do we use the data returned from the server?

 

let\'s open the console and see what does the following snippet return.

``` {.less}
let a = fetch("http://google.com");
```

Promises
========

Promises are the solution used in JS for when we don\'t want to **block
the program** while a  long running task is made.

 

By using promises, we create **asynchronous** code.

Promises
========

**fetch** uses **Promises** to work asynchronously.

 

**Promises** can be **pending**, **fulfilled** or **rejected**.

 

\- **pending**: the promise hasn\'t finished yet.

\- **fulfilled**: the promise finished correctly.

**- rejected**: there was an error in the promise

Promises
========

We use the methods **then** and **catch** to handle the different
outcomes of the promise (**fulfilled** and  **rejected** respectively)

``` {.less}
let a = fetch("https://google.com")

a.then((result) => console.log("the promise is fulfilled, and returned" + result))

a.catch((error) => console.log("the promise failed with " + error)
```

Back to fetch
=============

To get the JSON response from fetch we need to use promise\'s **then**
method:

``` {.less}
fetch("http://api.open-notify.org/iss-now.json")
  .then(data => data.json())
  .then(json => console.log(json))
```

Last day homework
=================

White belt
==========

Create a simple webpage in which, when a button is clicked, all the
links change their background to blue and their text color to white.

 

Blue belt
=========

Investigate the functional methods on array.  Namely **map**,
**filter**, **forEach**, and **reduce**.

Try to apply them to the following cases:

-   given an array of numbers, return only the **even ones**
-   given an array of numbers, return its **sum**
-   given an array of numbers, **log all** in the console
-   given an array of numbers, return a new array with **all elements
    squared**

 

Black belt
==========

Investigate about forms in HTML.

 

Create a **simple** web page in which the user can write the name of a
song in an **input** field and get the lyrics of that song.

 

You\'ll also need to investigate how to do HTTP requests from Javascript
(https://developer.mozilla.org/en-US/docs/Web/API/Fetch\_API/Using\_Fetch).

 

This is the API you\'ll need to use
https://lyricsovh.docs.apiary.io/\#reference/0/lyrics-of-a-song/search?console=1

 

Exercises
=========

Clone https://github.com/mcsbt-2019-web-and-mobile/session5-exercises

Exercises
=========

Let\'s review **server.py** together

Exercises
=========

Open **exercises.js**

Homework
========

There\'s no homework this week. There will be an individual assignment.
