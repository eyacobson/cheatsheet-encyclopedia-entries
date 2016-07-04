# HTML `<li>` Tag 

The HTML `<li>` tag represents a list item in an HTML document.

The `<li>` tag is a block element used to create list items within an ordered, or unordered list. An ordered list, which indents and numbers each item is created using the `<ol>` tag and an unordered list, which indents each item in the list and adds a bullet is created using the `<ul>` tag. List items can also occur within dir and menu tags which are created using the `<dir>` and `<menu>` tags. However, `<menu>` tag is only supported in Firefox, and it only works for context menus and the `<dir>` tag is not supported in HTML5. Lists are used quite commonly in HTML, apart from main page content, list can also come in handy when defining a website’s navigation.

## Syntax

The basic syntax of the `<li>` tag is as follows:

```
<li>This is a list item</li>
```

## Example 1

Here is a basic example that uses `<li>` tag within `<ul>` tag:

```
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

### Example Result:

<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

## Example 2

Here is a basic example that uses `<li>` tag within `<ol>` tag:

```
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>
```
### Example Result:

<ol>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ol>

## Example 3

You can create sub lists, or multilevel lists using `<li>` tags. This is achieved by embedding one list inside another:

```
<ul>
  <li>Top Level Item</li>
  <ul>
     <li>Mid Level Item 1
        <ul>
          <li>Sub-Item 1</li>
          <li>Sub-Item 2</li>
        </ul>
      </li>
     <li>Mid Level Item 2</li>
   </ul>
  <li>Top Level Item</li>
</ul>
```

### Example Result:

<ul>
  <li>Top Level Item</li>
  <ul>
     <li>Mid Level Item 1
        <ul>
          <li>Sub-Item 1</li>
          <li>Sub-Item 2</li>
        </ul>
      </li>
     <li>Mid Level Item 2</li>
   </ul>
  <li>Top Level Item</li>
</ul>

## Specific Attributes

The following table shows the attributes that are specific to the `<li>` tag:

Attribute | Value | Description
------------ | -------------- | -------------
type | "1" - Arabic numbers </br> "a" - Lowercase letters </br> "A" - Uppercase letters </br> "i" - Lowercase roman numerals </br> "I" - Uppercase roman numerals </br> "disk" - Disk </br> "square" - Square </br> "circle" - Circle | Specifies the numbering style for ordered lists and the bullet style for unordered lists. 
value | number | Specifies the number for the current list item (only for ordered lists).

**Note:** The "type" attribute is not supported in HTML5. You can use CSS style to define the type of list.

## Compatibility

The `<li>` tag is supported in all major modern browsers.

Chrome | IE | Firefox | Safari | Opera
------------ | ------------- | ------------- | ------------- | -------------
All versions | All versions | All versions | All versions | All versions

## Special Notes

A `<li>` tag will usually but not always contain text, it can also contain various block-level and inline-level elements, typically divs, span, p, nested ul or ol elements.  

If the `<li>` element is contained inside either of the `<dir>` and `<menu>` elements, it cannot contain block-level elements.
