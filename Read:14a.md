# Transforms

With CSS3 came new ways to position and alter elements. Now general layout techniques can be revisited with alternative ways to size, position, and change elements. All of these new techniques are made possible by the transform property. The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

# Transitions, and Animations:

One evolution with CSS3 was the ability to write behaviors for transitions and animations. Front end developers have been asking for the ability to design these interactions within HTML and CSS, without the use of JavaScript or Flash, for years. Now their wish has come true.

With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes. Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

![](https://camo.githubusercontent.com/6abdad437a7b0f001e709cd2c7eb588a2e7c812829460e4f3c1efac851bb8ce0/68747470733a2f2f747365332e6d6d2e62696e672e6e65742f74683f69643d4f49502e386673354273594d39775545642d4574725765436a414861466a267069643d41706926503d3026773d32333026683d313734)


## 2D Transforms
Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes.

Three-dimensional transforms work on both the x and y axes, as well as the z axis. These three-dimensional transforms help define not only the length and width of an element, but also the depth.

## 2D Rotate

The rotate value provides the ability to rotate an element from 0 to 360 degrees.

Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise.

The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically.

## 2D Scale

Using the scale value within the transform property allows you to change the appeared size of an element.

The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.

The scaleX value will scale the width of an element while the scaleY value will scale the height of an element.

To scale both the height and width of an element but at different sizes, the x and y axis values may be set simultaneously.

To do so, use the scale transform declaring the x axis value first, followed by a comma, and then the y axis value.

## 2D Translate

The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document.

Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.

As with the scale value, to set both the x and y axis values at once, use the translate value and declare the x axis value first, followed by a comma, and then the y axis value.

The distance values used within the translate value may be any general length measurement, most commonly pixels or percentages.

Positive values will push an element down and to the right of its default position while negative values will pull an element up and to the left of its default position.

## 2D Skew

The last transform value in the group, skew, is used to distort elements on the horizontal axis, vertical axis, or both.

The syntax is very similar to that of the scale and translate values. Using the skewX value distorts an element on the horizontal axis while the skewY value distorts an element on the vertical axis.

To distort an element on both axes the skew value is used, declaring the x axis value first, followed by a comma, and then the y axis value.%p

The distance calculation of the skew value is measured in units of degrees. Length measurements, such as pixels or percentages, do not apply here.

## Combining Transforms

It is common for multiple transforms to be used at once, rotating and scaling the size of an element at the same time for example. In this event multiple transforms can be combined together. To combine transforms, list the transform values within the transform property one after the other without the use of commas.

Using multiple transform declarations will not work, as each declaration will overwrite the one above it. The behavior in that case would be the same as if we were to set the height of an element numerous times. 

## Transform Origin

The transform-origin property can accept one or two values. When only one value is specified, that value is used for both the horizontal and vertical axes. If two values are specified, the first is used for the horizontal axis and the second is used for the vertical axis.