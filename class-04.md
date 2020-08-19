# Code 201

[PREVIOUS](https://dinaalsaid.github.io/reading-notes/class-03) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)  &nbsp; [NEXT](https://dinaalsaid.github.io/reading-notes/class-05)

## follow up

### links

using the **a** tag. ex: `<a href="URL">text the user clicks</a>`
used to linking pages togather or other websites.

* that there are two types of URLs : absolute (full website url) and relative (relative to the current page).
* to open links in a new window the target attribute in the anchor element is set to `_blank`.
* to link to a part of the page you can set the href value to the id of that element.
**Note** these can be combined to link to more specific places.

### layout

#### positioning

* normal flow :Every block element appears on a new line. which is the default for block elements.
* relative: block element is pushed down and right from where it would be in normal flow.
* absolute: This positions the element in relation to its containing element but does not affect the position of other surrounding elements.
* fixed: positions the element in relation to the browser window.
* floating: take an element out of normal flow and position it to the far left or right of a containing box.

you should have in mind that your website will appear on differnet devices with different screen width and resolution.(most designers design pages with 960-1000 pixel size).

### function expressions

If a function is put where the interpreter would expect to see an expression, then it is treated as an expression.also called an anonymous function.

ex:

```JavaScript
    var x = function (arg1, arg2){
        //code
        return value;
    };
```

in this example the expression expected is a value for the variable x,  instead a function is declared.

you can invoke the anonymous function imediately like this:

```JavaScript
    var x = (function (arg1, arg2){
        //code
        return value;
    } () ) ;
```

### variable scope

when declaring variable keep in mind the scope that they are going to be used in.
types of scopes:

* global
* local
Global variables use more memory. The browser has to remember them for as long as the web page using them is loaded. Local variables are only remembered during the period of time that a function is being executed (within their local scope)

### why is pair programming good

* Greater efficiency
* Engaged collaboration
* Learning from fellow students
* Social skills
* Job interview readiness
* Work environment readiness
