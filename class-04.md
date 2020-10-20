Read: 04 - Responsive Web Design and Regular Expressions

Grid Layout
The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats and positioning.
![i](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTbyHtYamLsu7pQN-mayfcB0UqIbJGeGGgWQQ&usqp=CAU)

``  display: grid;``

ou can adjust the gap size by using one of the following properties:

+ grid-column-gap
- grid-row-gap
+ grid-gap

Example
The grid-column-gap property sets the gap between the columns:

``.grid-container {``
``  display: grid;``
 `` grid-column-gap: 50px;``
``}``

The grid-gap property can also be used to set both the row gap and the column gap in one value:


``.grid-container {``
``  display: grid;``
 `` grid-gap: 50px;``
``}``



![io](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcTQOUnsAnsRU5Lj5HBwZ_8Q_eneJK7Oywbetg&usqp=CAU)

The grid-template-columns Property
The grid-template-columns property defines the number of columns in your grid layout, and it can define the width of each column.

The value is a space-separated-list, where each value defines the width of the respective column.

If you want your grid layout to contain 4 columns, specify the width of the 4 columns, or "auto" if all columns should have the same width.

Example
Make a grid with 4 columns:

``.grid-container {``
``  display: grid;``
 ``   grid-template-columns: auto auto auto auto;``
``}``

The justify-content Property
The justify-content property is used to align the whole grid inside the container.
![o](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRiFF-gjE556x4grAWhIWX05HgtJh5ouDn5gQ&usqp=CAU)

