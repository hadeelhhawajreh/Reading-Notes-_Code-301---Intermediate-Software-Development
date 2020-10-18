Read: 02 - jQuery, Events, and The DOM

![jq](https://zdnet1.cbsistatic.com/hub/i/2019/04/21/9d791bf2-9b20-476a-bba6-201e622d2a1f/jquery-logo-blue.png)



What You Should Already Know Before you start studying jQuery, you should have a basic knowledge of:

+ HTML
+ CSS
+ JavaScript

What is jQuery?
jQuery is a lightweight, "write less, do more", JavaScript library.

The purpose of jQuery is to make it much easier to use JavaScript on your website.

jQuery takes a lot of common tasks that require many lines of JavaScript code to accomplish, and wraps them into methods that you can call with a single line of code.

jQuery also simplifies a lot of the complicated things from JavaScript, like AJAX calls and DOM manipulation.

The jQuery library contains the following features:

HTML/DOM manipulation
CSS manipulation
HTML event methods
Effects and animations
AJAX
Utilities

Adding jQuery to Your Web Pages
There are several ways to start using jQuery on your web site. You can:

Download the jQuery library from jQuery.com
Include jQuery from a CDN, like Google
Downloading jQuery
There are two versions of jQuery available for downloading:

Production version - this is for your live website because it has been minified and compressed
Development version - this is for testing and development (uncompressed and readable code)
Both versions can be downloaded from jQuery.com.

The jQuery library is a single JavaScript file, and you reference it with the HTML ``<script>`` tag (notice that the ``<script>`` tag should be inside the ``<head>`` section):

``<head>``
``<script src="jquery-3.5.1.min.js"></script>``
``</head>``

Google CDN:
``<head>``
``<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>``
``</head>``

jQuery Syntax
The jQuery syntax is tailor-made for selecting HTML elements and performing some action on the element(s).

Basic syntax is: ``$(selector).action()``

A $ sign to define/access jQuery
A (selector) to "query (or find)" HTML elements
A jQuery action() to be performed on the element(s)

``$(this).hide() ``- hides the current element.

``$("p").hide() ``- hides all <p> elements.

``$(".test").hide() ``- hides all elements with class="test".

``$("#test").hide() ``- hides the element with id="test".

You might have noticed that all jQuery methods in our examples, are inside a document ready event:

``$(document).ready(function(){``

  ``// jQuery methods go here...``

``});``
This is to prevent any jQuery code from running before the document is finished loading (is ready).

It is good practice to wait for the document to be fully loaded and ready before working with it. This also allows you to have your JavaScript code before the body of your document, in the head section.

Here are some examples of actions that can fail if methods are run before the document is fully loaded:

Trying to hide an element that is not created yet
Trying to get the size of an image that is not loaded yet
Tip: The jQuery team has also created an even shorter method for the document ready event:

``$(function(){``

  ``// jQuery methods go here...``

``});``
