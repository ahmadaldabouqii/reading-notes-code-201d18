# Chart.js, Canvas

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

## What is HTML Canvas?
The HTML <canvas\> element is used to draw graphics, on the fly, via JavaScript.
The < anvas\> element is only a container for graphics. You must use JavaScript to actually draw the graphics.
Canvas has several methods for drawing paths, boxes, circles, text, and adding images.

## Basic usage of canvas

Let's start this tutorial by looking at the HTML element itself. At the end of this page, you will know how to set up a canvas 2D context and have drawn a first example in your browser. At first sight a looks like the  element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.

The id attribute isn't specific to the element but is one of the global HTML attributes which can be applied to any HTML element (like class for instance). It is always a good idea to supply an id because this makes it much easier to identify it in a script.

The element differs from an  tag in that, like for , , or elements, it is easy to define some fallback content, to be displayed in older browsers not supporting it, like versions of Internet Explorer earlier than version 9 or textual browsers. You should always provide fallback content to be displayed by those browsers.

## Drawing shapes with canvas

Browsers give us several ways to display graphics. The simplest way is to use styles to position and color regular DOM elements. This can get you quite far, as the game in the previous chapter showed. By adding partially transparent background images to the nodes, we can make them look exactly the way we want. It is even possible to rotate or skew nodes with the transform style.

But we’d be using the DOM for something that it wasn’t originally designed for. Some tasks, such as drawing a line between arbitrary points, are extremely awkward to do with regular HTML elements.

There are two alternatives. The first is DOM-based but utilizes Scalable Vector Graphics (SVG), rather than HTML. Think of SVG as a document-markup dialect that focuses on shapes rather than text. You can embed an SVG document directly in an HTML document or include it with an  tag.

The second alternative is called a canvas. A canvas is a single DOM element that encapsulates a picture. It provides a programming interface for drawing shapes onto the space taken up by the node. The main difference between a canvas and an SVG picture is that in SVG the original description of the shapes is preserved so that they can be moved or resized at any time. A canvas, on the other hand, converts the shapes to pixels (colored dots on a raster) as soon as they are drawn and does not remember what these pixels represent. The only way to move a shape on a canvas is to clear the canvas (or the part of the canvas around the shape) and redraw it with the shape in a new position.

![](https://camo.githubusercontent.com/b76ebe908a3be99ce097ce2ec9483d9c22041854b09bd662c4732000739c60fe/68747470733a2f2f63646e2d696d616765732d312e6d656469756d2e636f6d2f6d61782f3439302f312a545a515a36436f6d6c7276505a50487a30636a4462512e706e67)


## Applying styles and colors

In the chapter about drawing shapes, we used only the default line and fill styles. Here we will explore the canvas options we have at our disposal to make our drawings a little more attractive. You will learn how to add different colors, line styles, gradients, patterns and shadows to your drawings.

Colors Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

fillStyle = color Sets the style used when filling shapes. strokeStyle = color Sets the style for shapes’ outlines. color is a string representing a CSS , a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000).

Note: When you set the strokeStyle and/or fillStyle property, the new value becomes the default for all shapes being drawn from then on. For every shape you want in a different color, you will need to reassign the fillStyle or strokeStyle property.

The valid strings you can enter should, according to the specification, be CSS values. Each of the following examples describe the same color.

// these all set the fillStyle to ‘orange’

ctx.fillStyle = ‘orange’; ctx.fillStyle = ‘#FFA500’; ctx.fillStyle = ‘rgb(255, 165, 0)’; ctx.fillStyle = ‘rgba(255, 165, 0, 1)’; A fillStyle example In this example, we once again use two for loops to draw a grid of rectangles, each in a different color. The resulting image should look something like the screenshot. There is nothing too spectacular happening here. We use the two variables i and j to generate a unique RGB color for each square, and only modify the red and green values. The blue channel has a fixed value. By modifying the channels, you can generate all kinds of palettes. By increasing the steps, you can achieve something that looks like the color palettes Photoshop uses.