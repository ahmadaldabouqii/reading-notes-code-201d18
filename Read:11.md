# Images

Controlling the size and alignment of your images using CSS keeps rules that affect the presentation of your page in the CSS and out of the HTML markup.

You can control the size of an image using the width and height properties in CSS, just like you can for any other box. Specifying image sizes helps pages to load more smoothly because the HTML and CSS code will often load before the images, and telling the browser how much space to leave for an image allows it to render the rest of the page without waiting for the image to download. You might think that your site is likely to have images of all different sizes, but a lot of sites use the same sized image across many of their pages.

First you need to determine the sizes of images that will be used commonly throughout the site, then give each size a name. For example: small medium large Where the  elements appear in the HTML, rather than using width and height attributes you can use these names as values for the class attribute. In the CSS, you add selectors for each of the class names, then use the CSS width and height properties to control the image dimensions 

![](https://user-images.githubusercontent.com/79080942/111040728-1b404380-843d-11eb-9508-af4f54356455.png)


## Background-image

The background-image property allows us to place an image behind any HTML element.

## Background-repeat property can have four values:

* repeat
* repeat-x : The image is repeated horizontally only (as shown in the first example on the left).
* repeat-y: The image is repeated vertically only.
* no-repeat: The image is only shown once.
* fixed: The background image stays in the same position on the page.
* scroll: The background image moves up and down as the user scrolls up and down the page.

## Background position

* left top
* left center
* left bottom
* center top
* center center
* center bottom
* right top
* right center
* right bottom

# Video and Audio

## Video :
using <video\> tag you can add video to your page also:

1. controls :attribute adds video controls, like play, pause, and volume
2. width and height attributes can be included

## Audio :
using <audio\> tag you can add video to your page also:

1. controls :attribute adds video controls, like play, pause, and volume
2. Images can be aligned both horizontally and vertically using CSS.
3. You can use a background image behind the box created by any element on a page.
4. Background images can appear just once or be repeated across the background of the box.
5. You can create image rollover effects by moving the background position of an image.

Value	                 
* url('URL')	     >>         The URL to the image. To specify more than one image, separate the URLs with a comma
* none	      >>      No background image will be displayed. This is default
* linear-gradient()	>> Sets a linear gradient as the background image. Define at least two colors (top to bottom)
* radial-gradient() >>	Sets a radial gradient as the background image. Define at least two colors (center to edges)
* repeating-linear-gradient() >>	Repeats a linear gradient
* repeating-radial-gradient() >>	Repeats a radial gradient
* initial	>>  Sets this property to its default value. Read about initial
* inherit	>> Inherits this property from its parent element. Read about inherit

* To reduce the number of images your browser has to load, you can create image sprites.