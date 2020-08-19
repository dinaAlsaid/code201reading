# Code 201

[PREVIOUS](https://dinaalsaid.github.io/reading-notes/class-08) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)  &nbsp; [NEXT](https://dinaalsaid.github.io/reading-notes/class-10)

## forms

form controls:

* for adding text : text input, password input and textarea.
* for choices: checkboxes, radio buttons and drop down boxes.
* Submitting Forms: Submit buttons and Image buttons
* uploading files: File upload

form structure:

* action :the URL of the page where the info from the form is submitted to
* method : either get or post (post used for long forms and sensitive content)
* id

Labelling Form Controls using `<label>` tag where the for attribute is set to the id of the targeted input element.
grouping forms using `<fieldset>` and `<legend>`.

## Styling forms and lists

list-style-type controls the shape of the bulletpoints (or numeric style for ordered lists) used for the li element.
list-style-image can add an image as the points.
list-style-position can be inside the list element or outside it.
border-spacing, border-collapse used for defining Gaps Between Cells in tables
cursor to define the cursor shape (auto, crosshair, default, pointer,move,text,wait,help,url("cursor.gif");)

## events

event handling :

* select element to respond to
* which event is selected to trigger the response
* function when the event runs

three ways for event handling:

1. HTML event handlers (are not used today)
2. traditional DOM event handlers
3. level2 DOM event handlers (event listeners)

event flow:

1. capturing :from outside to inside
2. bubbling: from inside to outside (default)
