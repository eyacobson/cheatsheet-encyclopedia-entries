# CSS `border-radius` Property

The CSS `border-radius` property allows you to apply rounded corners to almost all HTML elements. It is used to specify the radius of the corners of an HTML element.

The `border-radius` property is a shorthand property for setting multiple `border radius` related properties in one place. It accepts up to four values and values represent, the `top-left`, `top-right`, `bottom-right`, and `bottom-left` corners. In other words, It is a shorthand property for the longhand properties: `border-top-left-radius`, `border-top-right-radius`, `border-bottom-right-radius`, and `border-bottom-left-radius`. 

## Syntax

**The formal syntax of the `border-radius` property is as follows:**

```
border-radius: [ <length> | <percentage> ]{1,4} [ / [ <length> | <percentage> ]{1,4} ]? 
```
The first set of (1-4) values define the horizontal radii for all four corners. An optional second set of values, preceded by a "/", define the vertical radii for all four corners. If only one set of values are supplied, these are used to determine both the vertical and horizontal equally.

**The informal syntax looks like this:**

````
border-radius: [radius value] [radius value]? [radius value]? [radius value]?;
````

In both cases, the question mark (?) means that the value is optional.

## Values

Every radius can be a `<length>` or `<percentage>` value. 

`<length>`: Specifies the radius using a fixed length. For example, 5px. Default value is 0.  
`<percentage>`: Specifies the radius using a percentage value. For example, 5%.

## Example 1

Here is a basic example that uses `border-radius` shorthand property:

```
border-radius: 10px;
border-radius: 20px 10px;
border-radius: 10px 25px 20px;
border-radius: 10px 20px 30px 40px;
```

### Example Result:  

![CSS Border Radius](http://www.monalighosh.com/LMD/border-radius1.jpg)

* If one value is given, then it specifies the radii of the four corners equally.
* If two values are given, then the first specifies the radii of the top-left and bottom-right corners, and the second value specifies the radii of the top-right and bottom-left corners. 
* If three values are given, the first specifies the radii of the top-left corner, the second specifies the radii of the top-right and bottom-left corners, and the third one specifies the radii of the bottom-right corner. 
* If four values are given, then they specify the radii of each of the four corners; that is, the first specifies the radii of the top-left corner, the second specifies the radii of the top-right corner, the third specifies the radii of the bottom-right corner, and the fourth one specifies the radii of the bottom-left corner.   

## Example 2

You can explicitly target individual corners of an element using the longhand syntax. For example:

```
border-top-right-radius: 20%;
```

### Example Result:

![CSS Border Radius](http://www.monalighosh.com/LMD/border-radius2.jpg)

## Example 3

You can also control the vertical and horizontal radii of each of the four corners by using this property. Look at the following example: 

```
border-radius: 108px 108px 108px 94px/128px 128px 128px 128px;
```

### Example Result:

![CSS Border Radius](http://www.monalighosh.com/LMD/border-radius3a.jpg)

The above diagram shows how this complex syntax really works. Here the values before the slash `/` apply to the horizontal radii of each corner, and the values after the slash apply to the vertical radii.

## Compatibility

The `border-radius` property is supported in all major modern browsers.

Chrome | IE | Firefox | Safari | Opera
------------ | ------------- | ------------- | ------------- | -------------
Version 4+ | Version 9+ | Version 4+ | Version 5+ | Version 10.5+

## Special Notes

While the border-radius property has now become widely supported in modern browsers and mobile devices, if you need to support older browsers you may want to use the vendor prefixes, `-webkit-border-radius` and `-moz-border-radius`. 

````
-webkit-border-radius: 5px;
-moz-border-radius: 5px;
border-radius: 5px;
````
The order of these rules is important. We define the webkit and mozilla rules first and then the border-radius rule. This is so that when this property finally becomes standardised, supporting browsers will use the final rule in this set and ignore the previous rules. 