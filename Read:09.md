# Forms 

## Why Forms?

The best known form on the web is probably
the search box that sits right in the middle of
Google's homepage.

## Form Controls

![](https://cdn.educba.com/academy/wp-content/uploads/2019/07/HTML-Form-Controls.png)

<br>

## Form Structure

* <form\>

    Form controls live inside a
    <form\> element. This element
    should always carry the action
    attribute and will usually have a
    method and id attribute too.

* action

    Every <form\> element requires
    an action attribute. Its value
    is the URL for the page on the
    server that will receive the
    information in the form when it
    is submitted.

* method

Forms can be sent using one of
two methods: get or post.
With the get method, the values
from the form are added to
the end of the URL specified in
the action attribute.

![](https://img.webnots.com/2014/01/How-HTML-Form-Works.png)

<br>

## Text Input

* <input\>

    The <input\> element is used
    to create several different form
    controls. The value of the type
    attribute determines what kind
    of input they will be creating.


* type="text"
    When the type attribute has a
    value of text, it creates a singleline text input.

* name
    When users enter information
    into a form, the server needs to
    know which form control each
    piece of data was entered into.
    (For example, in a login form, the
    server needs to know what has
    been entered as the username
    and what has been given as the
    password.) Therefore, each form
    control requires a name attribute.
    The value of this attribute
    identifies the form control and is
    sent along with the information
    they enter to the server.

* maxlength

    You can use the maxlength
    attribute to limit the number
    of characters a user may enter
    into the text field. Its value is the
    number of characters they may
    enter. For example, if you were
    asking for a year, the maxlength
    attribute could have a value of 4.

* Password Input

* <input\>
type="password"

    When the type attribute has
    a value of password it creates
    a text box that acts just like a
    single-line text input, except
    the characters are blocked out.
    They are hidden in this way so
    that if someone is looking over
    the user's shoulder, they cannot
    see sensitive data such as
    passwords.

* name

    The name attribute indicates
    the name of the password input,
    which is sent to the server with
    the password the user enters.

* size, maxlength
    It can also carry the size and
    maxlength attributes like the
    the single-line text input.

## Checkbox    

![](https://i0.wp.com/ao.gl/wp-content/uploads/2020/02/checkbox-optionen.png?fit=250%2C189&ssl=1)

> Whenever you want to collect information from
visitors you will need a form, which lives inside a
<form\> element.

> Information from a form is sent in name/value pairs.

> Each form control is given a name, and the text the
user types in or the values of the options they select
are sent to the server.

> HTML5 introduces new form elements which make it
easier for visitors to fill in forms.

> In addition to the CSS properties covered in other
chapters which work with the contents of all elements,
there are several others that are specifically used to
control the appearance of lists, tables, and forms.

> List markers can be given different appearances
using the list-style-type and list-style image
properties.

> Table cells can have different borders and spacing in
different browsers, but there are properties you can
use to control them and make them more consistent.

> Forms are easier to use if the form controls are
vertically aligned using CSS.

> Forms benefit from styles that make them feel more
interactive.

# Events

![](https://www.valentinog.com/blog/static/fae26592e45a4f01c6152c79b2cc5cee/c1b63/event-driven-nodejs-javascript.png)


## What is an Event ?

JavaScript's interaction with HTML is handled through events that occur when the user or the browser manipulates a page.

When the page loads, it is called an event. When the user clicks a button, that click too is an event. Other examples include events like pressing any key, closing a window, resizing a window, etc.

Developers can use these events to execute JavaScript coded responses, which cause buttons to close windows, messages to be displayed to users, data to be validated, and virtually any other type of response imaginable.

Events are a part of the Document Object Model (DOM) Level 3 and every HTML element contains a set of events which can trigger JavaScript Code.

Please go through this small tutorial for a better understanding HTML Event Reference. Here we will see a few examples to understand a relation between Event and JavaScript −


## onclick Event Type

This is the most frequently used event type which occurs when a user clicks the left button of his mouse. You can put your validation, warning etc., against this event type.


## onsubmit Event Type

onsubmit is an event that occurs when you try to submit a form. You can put your form validation against this event type.

> Events are the browser's way of indicating when
something has happened (such as when a page has
finished loading or a button has been clicked).

> Binding is the process of stating which event you are
waiting to happen, and which element you are waiting
for that event to happen upon.

> When an event occurs on an element, it can trigger a
JavaScript function. When this function then changes
the web page in some way, it feels interactive because
it has responded to the user.

> You can use event delegation to monitor for events
that happen on all of the children of an element.

> The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events. 

