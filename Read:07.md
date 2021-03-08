# Domain Modeling

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

# What's a Table?
![](https://www.mediumpedia.com/wp-content/uploads/2020/08/Create-Tables-in-HTML.png)

A table represents information in a grid format.
Examples of tables include financial reports, TV
schedules, and sports results.

## Basic Table Structure

* <table\>

    The <table\> element is used
    to create a table. The contents
    of the table are written out row
    by row.

* <tr\>

    You indicate the start of each
    row using the opening <tr\> tag.
    (The tr stands for table row.)
    It is followed by one or more
    <td\> elements (one for each cell
    in that row).
    At the end of the row you use a
    closing </tr\> tag.

* <td\>

    Each cell of a table is
    represented using a <td\>
    element. (The td stands for
    table data.)
    At the end of each cell you use a
    closing </td\> tag.

## Table Headings

* <th\>

    The <th\> element is used just
    like the <td\> element but its
    purpose is to represent the
    heading for either a column or
    a row. (The th stands for table
    heading.)
    Even if a cell has no content,
    you should still use a <td\> or
    <th\> element to represent
    the presence of an empty cell
    otherwise the table will not
    render correctly. (The first cell
    in the first row of this example
    shows an empty cell.)

## Long Tables

There are three elements that
help distinguish between the
main content of the table and
the first and last rows (which can
contain different content).
These elements help people
who use screen readers and also
allow you to style these sections
in a different manner than the
rest of the table (as you will see
when you learn about CSS).

*<thead\>

    The headings of the table should
    sit inside the <thead\> element.

* <tbody\>

    The body should sit inside the
    <tbody\> element.

* <tfoot\>

    The footer belongs inside the
    <tfoot\> element.

## Border & Background

The border attribute was used
on both the <table\> and <td\>
elements to indicate the width of
the border in pixels.

The bgcolor attribute was used
to indicate background colors
of either the entire table or
individual table cells. The value
is usually a hex code.

>
The <table\> element is used to add tables to a web
page.

> A table is drawn out row by row. Each row is created
with the <tr\> element.

> Inside each row there are a number of cells
represented by the <td\> element (or <th\> if it is a
header).

> You can make cells of a table span more than one row
or column using the rowspan and colspan attributes.

> For long tables you can split the table into a <thead\>,
<tbody\>, and <tfoot\>.

# WHAT IS AN OBJECT? 

Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.

## IN AN OBJECT: VARIABLES BECOME KNOWN AS PROPERTIES

If a variable is part of an object, it is called a
property. Properties tell us about the object, such as
the name of a hotel or the number of rooms it has.
Each individual hotel might have a different name
and a different number of rooms.

## IN AN OBJECT: FUNCTIONS BECOME KNOWN AS METHODS

If a function is part of an object, it is called a method.
Methods represent tasks that are associated with
the object. For example, you can check how many
rooms are available by subtracting the number of
booked rooms from the total number of rooms.

![](https://cdn-media-1.freecodecamp.org/images/fs6Q6b4ewNiWTuSehUQAY1Cf2OJTV0WyzHAB)

<br>

## CREATE & ACCESS OBJECTS CONSTRUCTOR NOTATION

![](https://cdn-images-1.medium.com/max/1024/1*GA7toY-Y3a3l0nlewOxIAw.png)

<br>

## WHAT ARE BUILT-IN OBJECTS?

Browsers come with a set of built-in objects that represent things like the
browser window and the current web page shown in that window. These
built-in objects act like a toolkit for creating interactive web pages. 

## THE BROWSER OBJECT MODEL: THE WINDOW OBJECT

The window object represents the current
browser window or tab. It is the topmost object
in the Browser Object Model, and it contains
other objects that tell you about the browser.

![](https://javascript.info/article/browser-environment/windowObjects.svg)

<br>

## USING THE BROWSER OBJECT MODEL

1. Two of the window object's
properties, i nnerWi dth and
i nnerHei ght, show width and
height of the browser window.

2. Child objects are stored as
properties of t heir parent object.
So dot notation is used to access
them, just like you would access
any other property of that object.

3. The element whose id
attribute has a value of info is
selected, and the message that
has been built up to this point is
written into the page.

![](https://1.bp.blogspot.com/-Z0QnE9eWAnM/XWj6B0TmfmI/AAAAAAAAZps/aRfAU517hg0ovfzgLUTZkmjHD3SXZCoWACLcBGAs/s640/DOM.PNG)

<br>

## THE DOCUMENT OBJECT MODEL: THE DOCUMENT OBJECT

The topmost object in the Document Object Model (or DOM) is the
document object. It represents the web page loaded into the current
browser window or tab.

![](https://eloquentjavascript.net/1st_edition/img/html.png)

<br>

## GLOBAL OBJECTS: NUMBER OBJECT

Whenever you have a value that is a number,
you can use the methods and properties of the
Number object on it.

* isNaN(); Checks if the value is not a number
* toFixed(); Rounds to specified number of decimal places (returns a string).
* toPrecision(); Rounds to total number of places (returns a string).
* toExponential(); Returns a string representing the number in exponential notation.

## GLOBAL OBJECTS: MATH OBJECT

The Math object has properties and methods
for mathematical constants and functions

* Math.PI Returns pi (approximately 3.14159265359).

* Math.round() Rounds number to the nearest integer.

* Math.sqrt(n) Returns square root of positive number, e.g., Math.sqrt(9) returns 3.

* Math.ceil() Rounds number up to the nearest integer.

* Math.floor() Rounds number down to the nearest integer.

* Math.random() Generates a random number between 0 (inclusive) and 1 (not inclusive).


> Functions allow you to group a set of related
statements together that represent a single task.

> Functions can take parameters (information required
to do their job) and may return a value.

> An object is a series of variables and functions that
represent something from the world around you.

> In an object, variables are known as properties of the
object; functions are known as methods of the object.

> Web browsers implement objects that represent both
the browser window and the document loaded into the
browser window.

> JavaScript also has several built-in objects such as
String, Number, Math, and Date. Their properties and
methods offer functionality that help you write scripts.

> Arrays and objects can be used to create complex data
sets (and both can contain the other). 

