Read: 01 - SMACSS and Responsive Web Design


![rwd](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTiYKtoF27b7BWNzaA_gUcy09CvFffIAYfcLQ&usqp=CAU)


## Responsive Web Design
With the growth in mobile Internet usage comes the question of how to build websites suitable for all users. The industry response to this question has become responsive web design, also known as **RWD.**

*Responsive Overview*
Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop. Responsive web design is focused around providing an intuitive and gratifying experience for everyone. Desktop computer and cell phone users alike all benefit from responsive websites.

- Responsive vs. Adaptive vs. Mobile
For some the term responsive may not be new, and others might be even more acquainted with the terms adaptive or mobile. Which may leave you wondering what exactly is the difference between all of them.

Responsive and adaptive web design are closely related, and often transposed as one in the same. Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change. With responsive design websites continually and fluidly change based on different factors, such as viewport width, while adaptive websites are built to a group of preset factors. A combination of the two is ideal, providing the perfect formula for functional websites. Which term is used specifically doesn’t make a huge difference.

Mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users. While this does occasionally have its place, it normally isn’t a great idea. Mobile websites can be extremely light but they do come with the dependencies of a new code base and browser sniffing, all of which can become an obstacle for both developers and users.



What is “Float”?
Float is a CSS positioning property. To understand its purpose and origin, we can look to print design. In a print layout, images may be set into the page such that text wraps around them as needed. This is commonly and appropriately called “text wrap”. Here is an example of that.

![float](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRS3MotZaBH2hti2qE6fSCIOsQbtIXCnrGjLg&usqp=CAU)

What are floats used for?
Aside from the simple example of wrapping text around images, floats can be used to create entire web layouts.


Flexible Grid
Let’s see how this formula works inside of a two column layout. Below we have a parent division with the class of container wrapping both the section and aside elements. The goal is to have have the section on the left and the aside on the right, with equal margins between the two. 

![grid](https://spyrestudios.com/wp-content/uploads/12-column-grids-structure.jpg)


Media Queries

Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example. Being able to apply uniquely targeted styles opens up a world of opportunity and leverage to responsive web design.

``@media all and (max-width: 1024px) {...}``

