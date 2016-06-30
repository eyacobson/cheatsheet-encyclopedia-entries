The `Math.exp()` Function
=========================

`Math.exp()` is a function in JavaScript. Similar functions are fundamental to
nearly all programming languages. Its purpose is to calculate Euler’s number,
`e`, raised to a given exponent.

All browser support this function.

 

Syntax
------

`Math.exp()` accepts one parameter: the exponent to which the base `e` is to be
raised. The syntax is therefore:

`Math.exp(exponent)`

 

Usage
-----

### Ex. 1

The basic usage of `Math.exp()` is as follows:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Math.exp(5)    //returns 148.413159103
Math.exp(0)    //returns 1
Math.exp(-2)   //returns 0.13533528323
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

 

### Ex. 2

Expressions of any degree of mathematical complexity may be written around this
function. It will be evaluated as an exponent using the traditional algebraic
order of operations. E.g.:

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
var A = 250 * Math.exp(0.046 * 1.5)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This calculates the expression:

250*e*\<sup\>(0.046)(1.5)\</sup\>, evaluating `Math.exp(0.046 * 1.5)` first, as
per order of operations. The result is `267.85905228708657`.

 

Special Notes
-------------

`Math.exp()` is not to be confused with `Math.pow()`. The latter supports the
syntax `Math.pow(base, exponent)`, allowing you to specify the base as well as
the exponent. In `Math.exp()`, the base is inherently always `e`.
