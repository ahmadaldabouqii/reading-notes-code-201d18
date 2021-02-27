# HTML Structure

>> HTML pages are text documents.

>> HTML uses tags (characters that sit inside angled brackets) to give the information they surround special
meaning.

## HTML Uses Elements to Describe the Structure of Pages ...

In the browser window you can see a web page that features exactly the same content as the Word document you met on the page 18. To describe the structure of a web page, we add code to the words we want to appear on the page.
You can see the HTML code for this page below. Don't worry about what the code means yet. We start to look at it in more detail on the next page. Note that the HTML code is in blue, and the text you see on screen is in black.

<br>

![i](https://i.stack.imgur.com/dmICu.png)

## Opening Tag & Closing Tag ...

Tags usually come in pairs. The opening tag denotes the start of a piece of content; the closing tag denotes the end.
Opening tags can carry attributes, which tell us more about the content of that element.


![i](https://clearlydecoded.com/assets/images/posts/2017-09-04-anatomy-of-html-tag/simple-p-tag.png)

<br>

## Atributes ..

Attributes provide additional information about the contents of an element. They appear on the opening tag of the element and are made up of two parts: a name and a value, separated by an equals sign.
Attributes require a name and a value.


![i](https://slideplayer.com/slide/16749469/97/images/13/ATTRIBUTES+TELL+US+MORE+ABOUT+ELEMENTS.jpg)

<br> 

# Extra Markup ..

## DOCTYPES

Because there have been several versions of HTML, each web page should begin with a DOCTYPE declaration to tell a browser which version of HTML the page is using (although browsers usually display the page even if it is not included).

![](https://www.seobility.net/en/wiki/images/a/a6/HTML-Doctype.png)

<br>

## Comments in HTML ...

If you want to add a comment
to your code that will not be
visible in the user's browser, you
can add the text between these
characters: 


![](https://amiradata.com/wp-content/uploads/2020/04/html-comments-e1586860890554.png)

<br>

## ID Attribute...

Every HTML element can carry
the id attribute. It is used to
uniquely identify that element
from other elements on the
page. Its value should start with
a letter or an underscore (not a
number or any other character).
It is important that no two
elements on the same page
have the same value for their id
attributes (otherwise the value is
no longer unique).

The id attribute is known as a
**global attribute** because it can
be used on any element.

![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2020/07/html-id-attribute-df.jpg)

<br>

## Class Attribute...

Every HTML element can
also carry a class attribute.
Sometimes, rather than uniquely
identifying one element within
a document, you will want a
way to identify several elements
as being different from the
other elements on the page.
The class attribute on any
element **can share the same
value, So, in this example, the
value of important could be
used on headings and links, too.**

![](https://www.wikitechy.com/css/img/css/css-class-selector.png)

<br>

## Block Elements && Inline Elements...

Some elements will always
appear to start on a new line in
the browser window. These are
known as block level elements.

![](https://puzzleweb.ru/en/images/html/type_el.png)

<br>

## Grouping Text & Elements In a Block...

The **<div\>** element allows you to group a set of elements together in one block-level box.

![](https://i.ytimg.com/vi/LMHqn7cK7xM/hqdefault.jpg)

<br>

## Grouping Text & Elements Inline...

### <span\>
The <span\> element acts like
an inline equivalent of the <div\>
element. It is used to either:
1. Contain a section of text
where there is no other suitable
element to differentiate it from
its surrounding text.
2. Contain a number of inline
elements.

The most common reason **why
people use <span\> elements**
is so that they can control the
appearance of the content of
these elements using CSS.

![](https://disenowebakus.net/en/images/articles/div-block-span-inline.jpg)

<br>

## IFrames...

An iframe is like a little window
that has been cut into your
page — and in that window you
can see another page. The term
iframe is an abbreviation of inline
frame.
One common use of iframes
(that you may have seen on
various websites) is to embed
a Google Map into a page. The
content of the iframe can be any
html page (either located on the
same server or anywhere else on
the web).

An iframe is created using the
<iframe\> element. There are a
few attributes that you will need
to know to use it: src, height, width, scrolling, frameborder, seamless.

![](https://cdn.shortpixel.ai/client/q_lossless,ret_img,w_750,h_410/https://www.floxblog.com/wp-content/uploads/2020/08/Auto-Adjust-HTML-iFrame-Height-According-to-its-Page-Contents-Height-Using-JavaScript-750x410.jpg)

<br>

## Information About Your Pages

### <meta\>

The <meta\> element lives
inside the <head\> element and
contains information about that
web page.
It is not visible to users but
fulfills a number of purposes
such as telling search engines
about your page, who created
it, and whether or not it is time
sensitive. (If the page is time
sensitive, it can be set to expire.)
The <meta\> element is an empty
element so it does not have a
closing tag. It uses attributes to
carry the information.

The value of the name attribute
can be anything you want it to
be. Some defined values for this
attribute that are commonly
used are:
description, keywords, robots.

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRxxNGBd_2wOFGDUGpEce75M4VzoeL6MkZLpQ&usqp=CAU)

<br>

# HTML5 Layout

## Traditional HTML Layouts...

For a long time, web page authors used <div\> elements to group
together related elements on the page (such as the elements that form a
header, an article, footer or sidebar). Authors used class or id attributes
to indicate the role of the <div\> element in the structure of the page.

![](https://i.pinimg.com/736x/36/ae/d0/36aed058a33efa95cc984eb277d410b0.jpg)

<br>

## Headers & Footers...

<header\> <footer\>

The <header\> and <footer\>
elements can be used for:
● The main header or footer
that appears at the top or
bottom of every page on the
site.
● A header or footer for an
individual <article\> or
<section\> within the page.

![](https://mobile.htmlgoodies.com/imagesvr_ce/1828/stylingblocks.png)

<br>

## Navigation...

<nav\>

The <nav\> element is used to
contain the major navigational
blocks on the site such as the
primary site navigation.

![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2020/07/HTML-Layout-df-1200x675.jpg)

<br>

## Articles...

<article\>

The <article\> element acts as
a container for any section of a
page that could stand alone and
potentially be syndicated.
This could be an individual
article or blog entry, a comment
or forum post, or any other
independent piece of content.
If a page contains several articles
(or even summaries of several
articles), then each individual
article would live inside its own
<article\> element.
The <article> elements can
even be nested inside each
other. For example, a blog post
might live inside one <article\>
element and each comment on
the article could live inside its
own child <article\> element.

![](https://www.w3resource.com/w3r_images/html5-atricle-image.png)

<br>

## Aside...
<aside\>

The <aside\> element has two
purposes, depending on whether
it is inside an <article\>
element or not.
When the <aside\> element
is used inside an <article\>
element, it should contain
information that is related to the
article but not essential to its
overall meaning. For example, a
pullquote or glossary might be
considered as an aside to the
article it relates to.
When the <aside\> element is
used outside of an <article\>
element, it acts as a container
for content that is related to
the entire page. For example,
it might contain links to other
sections of the site, a list of
recent posts, a search box, or
recent tweets by the author.

![](https://lh3.googleusercontent.com/proxy/Zr5vfysjCVLFd3hwwC-_9fsoC5Uo1oNlkaDnInfHFJk-0h4yy805tUD5Qlio3GjkujYTvn6H77NhRKDOx9tFAkrG1D4foZGvWeBd3fKKq8uWzQ)

<br>

## Heading Groups...
<hgroup\>

The purpose of the <hgroup\>
element is to group together a
set of one or more <h1\> through
<h6\> elements so that they are
treated as one single heading.
For example, the <hgroup\>
element could be used to contain
both a title inside an <h2\>
element and a subtitle within an
<h3\> element.

![](https://lh3.googleusercontent.com/proxy/_Hx40a-oEAjrtTife6LfqAVp9unyQ2I704Vq7xH-gFa-rHLl160JMg4hfMV-2rCW15QVxn-SyAtmp6R6AA4Q2asaPYuz9tTW_cSJ6YEM-lKui-eL6kMXnkowRx7iDQqcT80szAzgHYcqk56S)

<br>

## Figures...
<figure\> <figcaption\>

<figure\> It can be used
to contain any content that is
referenced from the main flow of
an article (not just images).
It is important to note that the
article should still make sense
if the content of the <figure\>
element were moved (to another
part of the page, or even to a
different page altogether).
For this reason, it should only be
used when the content simply
references the element (and not
for something that is absolutely
integral to the flow of a page).
Examples of usage include:
* Images
* Videos
* Graphs
* Diagrams
* Code samples
* Text that supports the main
body of an article

![](https://cdn.educba.com/academy/wp-content/uploads/2020/03/HTML-figure-Tag-Example-3-1.png)

>> Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements.

>> To make HTML5 elements work in Internet Explorer 8 (and older versions of IE), extra JavaScript is needed, which is available free from Google.

<br>

# Process & Design

## Site Maps...

The aim is to create a diagram
of the pages that will be used
to structure the site. This is
known as a **site map** and it will
show how those pages can be
grouped.
To help you decide what
information should go on each
page, you can use a technique
called **card sorting.**

![](https://mangools.com/blog/wp-content/uploads/2020/01/sitemap.png)

<br>

## WireFrames...

A wireframe is a simple sketch of the key
information that needs to go on each page of a site. It shows the hierarchy of the information and how much space it might require.

A lot of designers will take the
elements that need to appear on
each page and start by creating
wireframes. This involves
sketching or shading areas
where each element of the page
will go (such as the logo, primary
navigation, headings and main
bodies of text, user logins etc).

By creating a wireframe you can
ensure that all of the information
that needs to be on a page is
included.

![](https://d2slcw3kip6qmk.cloudfront.net/marketing/pages/chart/seo/wireframing/discovery/google-search-wireframe-updated-01.svg)

<br>

>> It's important to understand who your target audience is, why they would come to your site, what information they want to find and when they are likely to return.

>> Site maps allow you to plan the structure of a site.

>> Wireframes allow you to organize the information that will need to go on each page.

>> Design is about communication. Visual hierarchy helps visitors understand what you are trying to tell them.

>> You can differentiate between pieces of information using size, color, and style.

>> You can use grouping and similarity to help simplify the information you present.

<br>

# JAVA SCRIPT 

# What can we do with JavaScript?

![](https://www.internetacademy.co.in/_assets/img/what-you-can-do-with-javascript.jpg)

* *Access content.* You can use JavaScript to select any element, attribute, or text from an HTML page.
* *Modify Content.* You can use JavaScript to add or remove elements , attribute, or text to the page.
* *Program Rules.* You can specify a set of steps for the browser to follow.
* *React to Events.* You can specify that a script should run when a specific even has occured.

<br>

# Operators
**Expressions*** rely on things called ***operators***; they allow programmers to create a single value from one or more values. ***Several arithmetic operations*** can be performed in one expression, but it is importantto understand how the result will be calculated. Multiplication and division are performed before addition or subtraction. This can affect the number that you expect to see. To illustrate this effect, look at the following examples.

<br>

# WHAT IS A ***FUNCTION***?

**Functions** let you group a series of statements together to perform a specific task.
If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).
and is a very helpfull it's has many **benefits**:
- avoid duplicated.
- and it's reusable (created ones and use it many times).

<br>

# *WRITING A SCRIPT:*
To write a **script**, you need to first ***state your goal*** and then list the tasks that need to be completed in order to achieve it. Start with the big picture of what you want to achieve, and break that down into smaller **steps**:

>> ***DEFINE THE GOAL:*** First, you need to define the task you want to achieve. You can think of this as a puzzle for the computer to solve.

>> ***DESIGN THE SCRIPT:*** To design a script you split the goal out into a series of tasks that are going to be involved in solving this puzzle. This can be represented using a flowchart.

>> ***CODE EACH STEP:*** Each of the steps needs to be written in a programming language that the computer understands. In our case, this is JavaScript.

