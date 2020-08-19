# Code 201

[PREVIOUS](https://dinaalsaid.github.io/reading-notes/class-05) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)  &nbsp; [NEXT](https://dinaalsaid.github.io/reading-notes/class-07)

## Objects

objects are models that group a set of variables and functions to describe something in the real world.
variables inside an object are called properties.
functions inside an object are called methods.

### creating an object

```JavaScript
var obj1 ={
    pro1: val1,
    pro2: val2,

    method1: function(){
        //code here
    },
    method2: function(){
        //code here
    }
};
```

The properties and their values are called key-value pairs.
you can access the properties of the object two ways `obj1.pro1` or ``obj1['pro1']``
you can access the methods by ``obj1.method1()``

## Document Object Model (DOM)

The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.
As a browser loads a web page, it creates a model (DOM tree) of that page which consists of 4 nodes:

* Document nodes
* element nodes
* attribute nodes
* text nodes

### working with the DOM tree

1. access the elements: using the following queries:
    * getElementByld()
    * querySelector()
    * getElementsByClassName()
    * getElementsByTagName()
2. work with selected elements: using following methods:
    * innerHTML
    * textContent()
    * or the elements attributes.

If a method returns more than one element it returns something called a NodeList, which is similar to an array of objects.
There are two ways to select an element from a Nodelist:
The item() method and array syntax (more preferred because it is faster).
