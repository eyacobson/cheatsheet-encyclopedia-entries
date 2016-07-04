#  JavaScript `window.outerWidth` Property 

Javascript `window.outerWidth` property returns the total width of the browser window, including all interface elements of a window such as toolbars, scrollbars, window borders or the DevTools panel if you have it open and pinned to the side etc. This property is read-only and returns the width of the window in pixels. 

The `outerWidth` is one of the important properties of Javascript `Window` object which can be used when you are working on an app or a website that uses a lot of different sized windows and their sizes affect the user experience or when your script demands to get the width of your entire browser window, use the `window.outerWidth` property.

![JavaScript window.outerWidth](http://www.monalighosh.com/LMD/java-outerwidth.jpg)

## Syntax

The syntax of the `window.outerWidth` Property is as follows:

```
var totalWidth = window.outerWidth;
```

On return, `totalWidth` is the total width of the browser window.

## Example 1

Here is a basic example that uses `window.outerWidth` property to find out the total width of the browser window:

```
var totalWidth = window.outerWidth;
console.log("Width: " + totalWidth); 
```

### Example Result:

Width: 2560

## Compatibility

The `window.outerWidth` property is supported in all major modern browsers.

Chrome | IE | Firefox | Safari | Opera
------------ | ------------- | ------------- | ------------- | -------------
Version 1+ | Version 9+ | Version 1+ | Version 3+ | Version 9+

## Special Notes

The value of this property is read-only; if you want to change the dimensions of the browser window then you need to use available javascript resizing methods.

