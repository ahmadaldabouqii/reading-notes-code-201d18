# HTML Images

## Adding Images

<img\>

To add an image into the page
you need to use an <img\>
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:

> src

This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site.

> alt

This provides a text description
of the image which describes the
image if you cannot see it.

> title

You can also use the title
attribute with the <img\> element
to provide additional information
about the image. Most browsers
will display the content of this
attribute in a tootip when the
user hovers over the image.

![](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2020/07/html-images-df.jpg)

<br>

## Height & Width of Images

> height

This specifies the height of the
image in pixels.

> width

This specifies the width of the
image in pixels.

## Three Rules for Creating Images

1. Save images in the right format.
2. Save images at the right size.
3. Use the correct resolution.

<br>

## Image Formats: JPEG

![](https://www.remosoftware.com/info/wp-content/uploads/2018/03/JPG-vs-JPEG.jpg)

<br>

## Image Formats: GIF

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQpzCxTI65ear0PEXQS8Yeh2a5MURjGLPPY0g&usqp=CAU)

<br>

## HTML5: Figure and Figure Caption

<figure\>

Images often come with
captions. HTML5 has introduced
a new <figure\> element to
contain images and their caption
so that the two are associated.
You can have more than one
image inside the <figure\>
element as long as they all share
the same caption.

<figcaption\>

The <figcaption\> element has
been added to HTML5 in order
to allow web page authors to add
a caption to an image.
Before these elements were
created there was no way to
associate an <img\> element with
its caption.

<br>

# Color 

## Foreground Color

The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:

> RGB values

These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)

> hex codes

These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80

> color names

There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan

## CSS3: HSL & HSLA

The hsl color property has
been introduced in CSS3 as an
alternative way to specify colors.
The value of the property starts
with the letters hsl, followed
by individual values inside
parentheses for:

> hue

This is expressed as an angle
(between 0 and 360 degrees).

> saturation

This is expressed as a
percentage.

> lightness

This is expressed as a
percentage with 0% being white,
50% being normal, and 100%
being black.

The hsla color property allows
you to specify color properties
using hue, saturation, and
lightness as above, and adds a
fourth value which represents
transparency (just like the rgba
property). The a stands for:

> alpha

This is expressed as a
number between 0 and 1.0.
For example, 0.5 represents
50% transparency, and 0.75
represents 75% transparency.

> Color not only brings your site to life, but also helps
convey the mood and evokes reactions.

> There are three ways to specify colors in CSS:
RGB values, hex codes, and color names.

> Color pickers can help you find the color you want.

> It is important to ensure that there is enough contrast
between any text and the background color (otherwise
people will not be able to read your content).

> CSS3 has introduced an extra value for RGB colors to
indicate opacity. It is known as RGBA.

> CSS3 also allows you to specify colors as HSL values,
with an optional opacity value. It is known as HSLA.

<br>

# TEXT

> Serif 

    Serif fonts have extra details on
    the ends of the main strokes of
    the letters. These details are
    known as serifs.

> Sans-Serif

    Sans-serif fonts have straight
    ends to letters, and therefore
    have a much cleaner design.

> Monospace

    Every letter in a monospace (or
    fixed-width) font is the same
    width. (Non-monospace fonts
    have different widths.)


> Weight :  Light, Medium, Bold , Black     

> Style: Normal, Italic, Oblique.

> Stretch: Condensed, Regular, Extended.

<br>

## Size of Type

### font-size

> pixels

    Pixels are commonly used
    because they allow web
    designers very precise control
    over how much space their text
    takes up. The number of pixels is
    followed by the letters px.


> percentages

    The default size of text in
    browsers is 16px. So a size of
    75% would be the equivalent of
    12px, and 200% would be 32px.


## Units of Type Size

* Pixels
* Percentages 
* Ems