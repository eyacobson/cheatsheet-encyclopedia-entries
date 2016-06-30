The `outline-width` Property
============================

The `outline-width` CSS property sets the width of an outline around an element.
This property originated in CSS2.

An **outline** is a line that may be drawn around elements outside of their
borders. While it looks like a border, it is different from a border in the
following critical ways:

-   It invariably is drawn *around* the border, if one exists, never on top or
    in place of one.

-   It does not influence the position or size of the element it is around or of
    any other elements. Therefore, adding an outline, no matter how thick, can
    never change the flow of elements on the page.

-   Its thickness and styling must always be the same on all sides. Unlike
    borders, you cannot give specific styling to the top, bottom, left and right
    of an element’s outline.

 

Syntax
------

The syntax for `outline-width` is as follows:

`outline-width: medium | thin | thick | [length] | initial | inherit;`

 

### Values

`medium` -- A medium outline. **This is the default value.** It is typically
`3-4px` thick.

`thin` -- A thin outline. It is typically `1-2px` thick.

`thick` -- A thick outline. It is typically `5-6px` thick.

`[length]` -- Acceptable lengths may be specified in `px`, `pt`, or `em` units.
Percentages and negative values are not allowed.

`initial` -- Sets the property to its default value.

`inherit` -- Causes the property to be inherited from the parent element.
Inheritance for `outline-width` is **not** the default behavior, so it needs to
be explicitly invoked when needed using this value.

 

Usage
-----

### Ex. 1

The following CSS code will set an outline around a paragraph. Note that without
the accompanying use of `outline-style`, an outline will not appear, no matter
what width is specified.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
p {
    outline-width: thin;
    outline-style: solid;
    outline-color: black;
}
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

 

### Ex. 2

The following slightly more complex CSS example demonstrates clearly that an
outline surrounds a border, rather than replaces it. An outline is meant to
outline the entirety of an element, and a border is considered *part* of an
element.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
div {
    width: 200px;
    height: 200px;
    outline-width: 5px;
    outline-style: solid;
    outline-color: red;
    border: 5px solid black;
}
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This will result in a square with a black border and a red border (the outline)
around the black border. The width of the outline will not factor into the total
width of the element.

 

Special Notes
-------------

### Browser Compatibility

The `outline-width` property works on:

-   Chrome 1.0+

-   Internet Explorer 8.0+

-   Firefox 1.5+ (browsers prior to v. 1.5 should use `moz-outline-width`)

-   Safari 1.2+

-   Opera 7.0+

### Special Bugs

-   **In IE8 for Windows:** When a parent element has `text-align: justify;`
    applied to it, then the outline around inline elements within that parent
    will be drawn around the position those elements would have been in had
    `justify` not been used. This will cause the outline and those elements to
    be misaligned.

-   **In Firefox 3.5 & below:** When content overflows its boundaries, an
    outline would get drawn around all of the overflow as well, rather than
    remaining around the element’s actual set / intended dimensions.
