# Code 201

[PREVIOUS](https://dinaalsaid.github.io/reading-notes/class-07) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)  &nbsp; [NEXT](https://dinaalsaid.github.io/reading-notes/class-09)

## CSS layout

* block elements: start on a new line
* inline elements: flow in between surrounding text

If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

### changing the element position

* normal flow: `position:static`
* Relative : `position:relative`
* Absolute: `position:absolute`
* fixed: `position:fixed`
* sticky: `position:sticky`

you can control overlapping elements by assigning the z-index attribute to integer values, which determines what elements are placed above other elements when they overlap.

float can be used to display elements side by side.

### fixed and liquid layouts

liquuid layouts change the dimension of the boxes relative to another element (%) or to default dimensions (em and rem).
for fixed layouts, pixels, points, inches, and cm are used to determine dimensions of boxes.
