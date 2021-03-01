# TEXT in HTML

In this chapter we focus on how to add markup to the text that
appears on your pages. You will learn about:
* Structural markup: the elements that you can use to describe both headings and paragraphs
* Semantic markup: which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the
meaning of acronyms, and so on.

<br>

## Headings
<hr>
* HTML has six "levels" of
headings:
<h1\>
<h2\>
<h3\>
<h4\>
<h5\>
<h6\>

Browsers display the contents of
headings at different sizes. The
contents of an <h1\> element is
the largest, and the contents of
an <h6\> element is the smallest.
The exact size at which each
browser shows the headings
can vary slightly. Users can also
adjust the size of text in their
browser. You will see how to
control the size of text, its color,
and the fonts used when we
come to look at CSS.

![](https://www.schudio.com/wp-content/uploads/2016/10/html-headings.png?x97747)

<br>

## Paragraphs
<hr>
<p\>
To create a paragraph, surround
the words that make up the
paragraph with an opening <p\>
tag and closing </p\> tag.

![](https://cdo-curriculum.s3.amazonaws.com/media/uploads/html_element.png)

<br>

## Bold & Italic
<hr>

![het](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQlkFi5HaoQLebfzSD0xF_2dECzvphCstrapw&usqp=CAU)

<br>

## Superscript & Subscrip
<hr>
The <sup\> element is used
to contain characters that
should be superscript such
as the suffixes of dates or
mathematical concepts like
raising a number to a power such
as 22.

The <sub\> element is used to
contain characters that should
be subscript. It is commonly
used with foot notes or chemical
formulas such as H2
0.

![](https://support.content.office.net/en-us/media/0e396025-76a9-4051-8960-74ca0aeeb739.png)

<br>

## White Space
<hr>
In order to make code easier to
read, web page authors often
add extra spaces or start some
elements on new lines.
When the browser comes across
two or more spaces next to each
other, it only displays one space.
Similarly if it comes across a line
break, it treats that as a single
space too. This is known as
white space collapsing.

<br/>
<br/>

## Line Breaks & Horizontal Rules
<hr>

<br/\>
As you have already seen, the
browser will automatically show
each new paragraph or heading
on a new line. But if you wanted
to add a line break inside the
middle of a paragraph you can
use the line break tag <br\/>.

<hr\/>
To create a break between
themes — such as a change of
topic in a book or a new scene
in a play — you can add a
horizontal rule between sections
using the <hr\/> tag.

![](https://raw.githubusercontent.com/lennyroyroy/basics-image/master/linebreak-horizontal.png)

<br>

# Semantic Markup

There are some text elements that are not intended to affect the
structure of your web pages, but they do add extra information to the
pages — they are known as semantic markup.

![](https://cdn.hallme.com/uploads/semantic-markup.png)

<br>

## Strong & Emphasis
<hr>

<strong\>

The use of the <strong\>
element indicates that its
content has strong importance.
For example, the words
contained in this element might
be said with strong emphasis.
By default, browsers will show
the contents of a <strong\>
element in bold.

<em\>

The <em> element indicates
emphasis that subtly changes
the meaning of a sentence.
By default browsers will show
the contents of an <em\> element
in italic.

<br>

## Abbreviations & Acronyms
<hr>

<abbr\>

If you use an abbreviation or
an acronym, then the <abbr\>
element can be used. A title
attribute on the opening tag is
used to specify the full term.

In HTML 4 there was a separate
<acronym\> element for
acronyms. To spell out the full
form of the acronym, the title
attribute was used (as with the
<abbr\> element above). HTML5
just uses the <abbr\> element
for both abbreviations and
acronyms.


![](https://miro.medium.com/max/1200/1*1scHN4FpWnMNepfv6BtJXA.png)

<br>

## Citations & Definitions
<hr>

<cite\>
When you are referencing a
piece of work such as a book,
film or research paper, the
<cite\> element can be used
to indicate where the citation is
from.
In HTML5, <cite\> should not
really be used for a person's
name — but it was allowed in
HTML 4, so most people are
likely to continue to use it.

<dfn\>
The first time you explain some
new terminology (perhaps an
academic concept or some
jargon) in a document, it is
known as the defining instance
of it.
The <dfn\> element is used to
indicate the defining instance of
a new term.

![](https://study.com/cimages/videopreview/videopreview-full/y46v2bw1zb.jpg)

<br>

## Author Details
<hr>

<address\>

The <address\> element has
quite a specific use: to contain
contact details for the author of
the page.
It can contain a physical address,
but it does not have to. For
example, it may also contain a
phone number or email address.

<br>

## Changes to Content
<hr>

<ins\><del\>

The <ins\> element can be used
to show content that has been
inserted into a document, while
the <del\> element can show text
that has been deleted from it.

<s\>

The <s\> element indicates
something that is no longer
accurate or relevant (but that
should not be deleted).

<br>

> HTML elements are used to describe the structure of the page (e.g. headings, subheadings, paragraphs).

> They also provide semantic information (e.g. where emphasis should be placed, the definition of any
acronyms used, when given text is a quotation).

# Introducing CSS

> CSS Associates Style rules with HTML
elements

![](https://www.bitdegree.org/learn/storage/media/images/css-tutorial-img1-01.o.png)

<br>

CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a **selector** and a **declaration**.


![](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/CSS_basics/css-declaration-small.png)

## Using External CSS
<hr>

<link\>

The <link\> element can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page. It is an
empty element (meaning it does
not need a closing tag), and it
lives inside the <head\> element.
It should use three attributes:
* **href**

    This specifies the path to the
    CSS file (which is often placed in
    a folder called css or styles).

* **type***

    This attribute specifies the type
    of document being linked to. The
    value should be text/css.

* **rel**

    This specifies the relationship
    between the HTML page and
    the file it is linked to. The value
    should be stylesheet when
    linking to a CSS file.

<br>

![](https://www.wikitechy.com/css/img/css/css-external-stylesheet.png)

<br>

# JavaScript Introduction

## STATEMENTS 
<hr>

A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon.

![](https://cdn.programiz.com/sites/tutorial2program/files/js-if-else-statement.png)

<br>

## COMMENTS 
<hr>

You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code. 

![](https://lh3.googleusercontent.com/proxy/ngms9nG_-7g2AWAWYCHKqFsXZPdDlpB1Qby1QvIixa0bfqXcF0St9vNq6UJPPv-NBro1I6PYrDND1vsQz9EQdCgQnYRVwfqBqOOjOW4pasVxZVqahsGfkR8IKxBiX-PiwO7mfnC62WHz6WqSnEEJylBqmP3ZOHtlecvIWDvuMM64z3nIKaamw5Yca0mmW9mWDCNR80rt7R7LCvSH4N794FJo56N8dHsq8gs)

<br>

## WHAT IS A VARIABLE? 
<hr>

A script will have to temporarily
store the bits of information it
needs to do its job. It can store this
data in variables.


![](https://www.tutsmake.com/wp-content/uploads/2020/05/JavaScript-Variable-Example.jpeg)

<br>

## DATA TYPES 
<hr>

![](https://i.morioh.com/2020/04/06/656042698c06.jpg)

* NUMERIC DATA TYPE

    The numeric data type handles
    numbers. like:
    0.75

* STRING DATA TYPE 

    The strings data type consists of letters and other characters. like:
    "Hey Im String"

* BOOLEAN DATA TYPE 
    Boolean data types can have one
of two values: **true or false**.


<br>

## ARRAYS
<hr>

An array is a special type of variable. It doesn't
just store one value; it stores a list of values. 

![](https://ko.javascript.info/article/arraybuffer-binary-arrays/arraybuffer-views.svg)

<br>

## 
<hr>

* Operation conditions…

    >    == egual to

    >    != not equal to

    >   === strict equal to
    
    >    !=== strict not equal to

    >    (>) greater than

    >    (<) less than

    >    (>=) greater than or equal

    >    <= less than or equal


* The summary of Comparison and logical operators…

    >   Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>).

    >   are used to compare two operands.

    >   Logical operators allow you to combine more than one.

    >   set of comparison operators.

    >   if … else statements allow you to run one set of code.

    >   if a condition is true, and another if it is false.
    
    >   switch statements allow you to compare a value.

    >   against possible outcomes (and also provides a default option if none match).

    >   Data types can be coerced from one type to another.

    >   All values evaluate to either truthy or falsy. There are three types of loop:   for, while, and do … while. Each repeats a set of statements.


## WORKING WITH DATES & TIMES
<hr>

* To specify a date and time, you
can use this format:

    YYYY, MM, OD, HH, MM, SS
    1996, 04, 16, 15, 45 , 55
    This represents 3:45pm and 55
    seconds on April 16, 1996.

* The order and syntax for this is:

    Year      >      four digits
    
    Month      >     0-11 (Jan is 0)

    Day        >     1-31

    Hour       >     0-23

    Minutes    >     0-59

    Seconds     >    0-59S

    Milliseconds  >  0-999 


![](https://i.ytimg.com/vi/CnozSz4wbBQ/maxresdefault.jpg)

<br>

## SWITCH STATEMENTS 
<hr>

A switch statement starts with a
variable called the switch value.
Each case indicates a possible
value for this variable and the
code that should run if the
variable matches that value.

![](https://cdn.javascripttutorial.net/wp-content/uploads/2016/08/JavaScript-switch-case.png)

<br>

## USING DO WHILE LOOPS 
<hr>

The key difference between
a whi 1 e loop and a do whi 1 e
loop is that the statements in
the code block come before the
condition. This means that those
statements are run once whether
or not the condition is met.

If you take a look at the
condition, it is checking that the
value of the variable called i is
less than 1, but that variable has
already been set to a value of 1.

Therefore, in this example the
result is that the 5 times table is
written out once, even though
the counter is not less than 1.

![](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/JavaScript-Loops-1200x675.jpg)

<br>

> There are three types of loop: for, while, and
do ... while. Each repeats a set of statements.