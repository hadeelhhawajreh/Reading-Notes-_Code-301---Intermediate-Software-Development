Readings: SENDING FORM DATA

Client/server architecture
At it's most basic, the web uses a client/server architecture that can be summarized as follows. a client (usually a web browser) sends a request to a server (most of the time a web server like Apache, Nginx, IIS, Tomcat, etc.), using the HTTP protocol. The server answers the request using the same protocol.

![o](https://media.prod.mdn.mozit.cloud/attachments/2012/11/20/4291/c1a4a06f1fd9ed42ec5b06e814dd3111/client-server.png)
The <form> element defines how the data will be sent. All of its attributes are designed to let you configure the request to be sent when a user hits a submit button. The two most important attributes are action and method.

>The action attribute
The action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. If this attribute isn't provided, the data will be sent to the URL of the page containing the form — the current page.


`` <form action="https://example.com"> ``

The method attribute

The method attribute defines how data is sent. The HTTP protocol provides several ways to perform a request; HTML form data can be transmitted via a number of different methods, the most common being the GET method and the POST method

To understand the difference between those two methods, let's step back and examine how HTTP works. Each time you want to reach a resource on the Web, the browser sends a request to a URL. An HTTP request consists of two parts: a header that contains a set of global metadata about the browser's capabilities, and a body that can contain information necessary for the server to process the specific request.

![podt and get](https://techdifferences.com/wp-content/uploads/2018/06/Get-vs-Post.jpg)


The GET method

The GET method is the method used by the browser to ask the server to send back a given resource: "Hey server, I want to get this resource." In this case, the browser sends an empty body. Because the body is empty, if a form is sent using this method the data sent to the server is appended to the URL.

The POST method

The POST method is a little different. It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request: "Hey server, take a look at this data and send me back an appropriate result." If a form is sent using this method, the data is appended to the body of the HTTP request.

Let's look at an example — this is the same form we looked at in the GET section above, but with the method attribute set to POST.


Forms in HTML5
The HTML elements that allow you to build interactive forms

![p](https://www3.ntu.edu.sg/home/ehchua/programming/webprogramming/images/JS_FormValidation.png)


Type: Inline
Self-closing: No
Permalink
Share
MDN
#button
Defines a clickable button.

Example:
Copy
Submit form
<button>
  Submit form
</button>
name
Defines the unique identifier for that button within the form. It allows the server to access each button's value when submitted.

"submit_button"
The name value must be unique within the context of a <form> container.

It can only contain alphanumeric characters a-z A-Z 0-9 and some special characters like - _… but no space.

Submit form
value
The value sent to the server when submitting the form.

"primary"
The server will receive the value primary.

type
Defines the button type.

"submit"
The button sends the form data to the server.

"reset"
The button resets the form.

disabled
Disables the button.

autofocus
Sets focus on the element when the web page loads.

fieldset
Defines a group of controls within a form.

legend
Defines a caption for a parent's content.
