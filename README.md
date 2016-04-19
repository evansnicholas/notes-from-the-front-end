# Notes from the front-end

This is a collection of notes concerning front-end web-development, initially
inspired by discussions that took place during a front-end themed reading group.
Front-end development is interpreted broadly as encompassing all the skills
involved in the production of a top-notch web experience: browser development,
native mobile development, UX Design and API design.  

## Developing for the browser

Browser development is based on the following three fundamental technologies:
1. HTML
2. CSS
3. Javascript

### HTML

### CSS

### Javascript

Javascript was initially introduced by Netscape.  Several other browsers
introduced similar scripting languages, and an attempt was made at writing a
unifying specification called ECMA Script.  The languages evolved faster than
the specification.

ECMA script is only the language and says nothing about the environment in which
the language is embedded.  The browser is one such environment and it adds
API's known as the DOM (Document Object Model) and the BOM (Browser Object Model).
These API's are not part of the ECMA script specification, instead they are
specified as part of HTML5 (this makes HTML5 far more than a markup language).

The integration of javascript in HTML documents has evolved.  Some sites include many script tags in a page, and careful attention must be payed to script loading
characteristics. These can be controlled by the script tag attributes _async_ and
_defer_.  

HTML pages are a combination of many different technologies (HTML, CSS, javascript,
other markup languages such as SVG or MathML...).  XHTML was an initial attempt to
formalize how all these technologies fit together and provide strict validation of
HTML pages.  However, this approach has fallen by the way side and has been replaced
by HTML 5.    

Javascript has 5 basic types:
+ String
+ Number
+ Boolean
+ null
+ undefined

_undefined_ should never be used explicitly in code, it is a type that is returned when things go wrong (for instance when an attempt is made to access a non-existent object property). In code, _null_ can be used to express an empty object reference.  

Javascript incorporates many implicit conversions between types.  These implicit conversions take place when certain operators are used, such as mathematical operations, and most importantly the equality operator == .  These implicit conversions are very confusing and should be avoided.  Javascript does also provide ways to avoid these implicit conversions.  For instance the === operator compares arguments without first coercing the types.  The _switch_ statement also choses its branch by using the === operator.

In ES5 there is no block scope.  Var declarations inside a block are "hoisted" outside to the enclosing scope.  This situation in improved in ES6 by the let operator, which does respect block scope.

Javascript is a garbage collected language.  Most implementations use a mark and sweep garbage collection strategy.  




#### References

+ Nicholas Zakas, _Professional Javascript for Web Developers_

+ [MDN HTML5](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)


## Native mobile development

## UX Design

## API Design
