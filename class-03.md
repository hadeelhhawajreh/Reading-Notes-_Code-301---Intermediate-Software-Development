Readings: MUSTACHE and FLEXBOX

**Javascript Templating**
![img](https://miro.medium.com/max/875/1*P9q0tkeaRY2l1JOXaVKAig.png)
 
Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.
The template engine then replaces variables and instances declared in a template file with actual values at runtime, and convert the template into an HTML file sent to the client.
Mustache

Javascript Templating
Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.
The template engine then replaces variables and instances declared in a template file with actual values at runtime, and convert the template into an HTML file sent to the client.
Mustache



![img](https://miro.medium.com/max/875/1*LbqYj87xlazySm6wE0Q2lA.png)


FLEXBOX
display
This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.

![img](https://css-tricks.com/wp-content/uploads/2018/10/01-container.svg)
flex-direction
the four possible values of flex-direction being shown: top to bottom, bottom to top, right to left, and left to right

This establishes the main-axis, thus defining the direction flex items are placed in the flex container. Flexbox is (aside from optional wrapping) a single-direction layout concept. Think of flex items as primarily laying out either in horizontal rows or vertical columns.

+ row (default): left to right in ltr; right to left in rtl
+ row-reverse: right to left in ltr; left to right in rtl
+ column: same as row but top to bottom
+ column-reverse: same as row-reverse but bottom to top


 flex-wrap: 
 
+ nowrap (default): all flex items will be on one line
+ wrap: flex items will wrap onto multiple lines, from top to bottom.
+ wrap-reverse: flex items will wrap onto multiple lines from bottom to top.

ORDER
By default, flex items are laid out in the source order. However, the order property controls the order in which they appear in the flex container
``  order: 5; /* default is 0 */``



This defines the alignment along the main axis. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. It also exerts some control over the alignment of items when they overflow the line.

.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly | start | end | left | right ... + safe | unsafe;
}
flex-start (default): items are packed toward the start of the flex-direction.
flex-end: items are packed toward the end of the flex-direction.
start: items are packed toward the start of the writing-mode direction.
end: items are packed toward the end of the writing-mode direction.
left: items are packed toward left edge of the container, unless that doesn’t make sense with the flex-direction, then it behaves like start.
right: items are packed toward right edge of the container, unless that doesn’t make sense with the flex-direction, then it behaves like start.
center: items are centered along the line
space-between: items are evenly distributed in the line; first item is on the start line, last item on the end line
space-around: items are evenly distributed in the line with equal space around them. Note that visually the spaces aren’t equal, since all the items have equal space on both sides. The first item will have one unit of space against the container edge, but two units of space between the next item because that next item has its own spacing that applies.
space-evenly: items are distributed so that the spacing between any two items (and the space to the edges) is equal.
Note that that browser support for these values is nuanced. For example, space-between never got support from some versions of Edge, and start/end/left/right aren’t in Chrome yet. MDN has detailed charts. The safest values are flex-start, flex-end, and center.

There are also two additional keywords you can pair with these values: safe and unsafe. Using safe ensures that however you do this type of positioning, you can’t push an element such that it renders off-screen (e.g. off the top) in such a way the content can’t be scrolled too (called “data loss”).
![img2](https://css-tricks.com/wp-content/uploads/2018/10/justify-content.svg)
