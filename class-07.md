# Code 201

[PREVIOUS](https://dinaalsaid.github.io/reading-notes/class-06) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)  &nbsp; [NEXT](https://dinaalsaid.github.io/reading-notes/class-08)

## tables  in HTML

how to create a table.

* `<table>`: contains the tags that build our table.
* `<tr>`: define a row
* `<td>`: add row cell with data
* `<th>`: used to add heading to our table
* `<td colspan=”2”>`: to make the cell take 2 cols space (can be done with rowspan too)

## Objects

another way of creating object is:

```JavaScript
var name = new Object();
    name.prop1: val1,
    //..etc.

```

## Constructors

are functions that are called when the object is created, it can set default values for the object properties or invoke the object methods.
creating an object with a constructor

```JavaScript
function Object1(Prop1,prop2) {
  this.prop1 = val1;
  this.prop2 = val2;
  this.method1 = function(){
      //code here
  };
};
```  
