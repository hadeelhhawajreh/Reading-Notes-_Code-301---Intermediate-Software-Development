Read: 11 :EJS

![IMG](https://miro.medium.com/max/720/1*DG4VA127mu4Fx2TrRIzskw.jpeg)



``<%= EJS %>``
Embedded JavaScript templating.

*What is EJS?*
What is the "E" for? "Embedded?" Could be. How about "Effective," "Elegant," or just "Easy"? EJS is a simple templating language that lets you generate HTML markup with plain JavaScript. No religiousness about how to organize things. No reinvention of iteration and control-flow. It's just plain JavaScript.

> Simple template tags:`` <% %>``

Use
Pass EJS a template string and some data. BOOM, you've got some HTML.

``let ejs = require('ejs');``
``let people = ['geddy', 'neil', 'alex'];``
``let html = ejs.render('<%= people.join(", "); %>', {people: people});``

> Browser support
Download a browser build from the latest release, and use it in a script tag.

 ``<script src="ejs.js"></script>``
``<script>``
  ``let people = ['geddy', 'neil', 'alex'];``
  ``let html = ejs.render('<%= people.join(", "); %>', {people: people});``
``</script>``

Example :
    ``<% if (user) { %>``
     ``<h2><%= user.name %></h2>``
``<% } %>``


> Tags

``<% 'Scriptlet' tag, for control-flow, no output``
``<%_ ‘Whitespace Slurping’ Scriptlet tag, strips all whitespace before it``
``<%= Outputs the value into the template (HTML escaped)``
``<%- Outputs the unescaped value into the template``
``<%# Comment tag, no execution, no output``
``<%% Outputs a literal '<%'``
``%> Plain ending tag``
``-%> Trim-mode ('newline slurp') tag, trims following newline``
``_%> ‘Whitespace Slurping’ ending tag, removes all whitespace after it``


> Includes

Includes are relative to the template with the include call. (This requires the 'filename' option.) For example if you have "./views/users.ejs" and "./views/user/show.ejs" you would use <%- include('user/show'); %>.

You'll likely want to use the raw output tag (<%-) with your include to avoid double-escaping the HTML output.

``<ul>``
  ``<% users.forEach(function(user){ %>``
    ``<%- include('user/show', {user: user}); %>``
  ``<% }); %>``
``</ul>``
