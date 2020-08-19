# Code 201

[PREVIOUS](https://dinaalsaid.github.io/reading-notes/class-13) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)  &nbsp; [NEXT](https://dinaalsaid.github.io/reading-notes/class-14b)

## transfroms

the transform property comes in two different settings, two-dimensional and three-dimensional and is used to control the positionof elements in a more advanced way than the traditional methods.

To enhance support across browsers the transform property has many prefixes:

```CSS
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```

### 2D transforms

1. The `rotate` value provides the ability to rotate an element from 0 to 360 degrees.(The default point of rotation is the center of the element)
ex:

```css
.box-1 {
  transform: rotate(20deg);
}
```

2. Using the `scale` value allows you to change the appeared size of an element. (1 represents the original size).
`scaleX` is used to scale the width of the element. `scaleY`, the height.

```css
.box-3 {
  transform: scale(.5, 1.15);
}
```

3. `translate` value pushes and pulls an element in different directions without interrupting the normal flow of the document.

ex:

```css
.box-3 {
  transform: translate(-10px, 25%);
}
```

4. `skew` is used to distort elements on the horizontal axis, vertical axis, or both.
all these can be combined for desired effects. also the origin point can be moved using `transform-origin: X Y`

## trnasitions

for a transition to take place, an element must have a change in state, and different styles must be identified for each state.The easiest way for changing styles for different states is by using pseudo-classes.(:hover, :focus, :active, and :target )

1. transition-property, selects the property that's changing
2. transition-duration: how long does the transition take
3. transition-timing-function:  used to set the speed in which a transition will move.(linear ease-in ease-out ease-in-out)
4. transition-delay: after how much time the transition should start 

ex:

``` css
.box {
  background: #2db34a;
  border-radius: 6px;
  transition-property: background, border-radius;
  transition-duration: .2s, 1s;
  transition-timing-function: linear, ease-in;
}
.box:hover {
  background: #ff7b29;
  border-radius: 50%;
}
```

## animations

To set multiple points at which an element should undergo a transition, use the `@keyframes` rule.
The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

ex:

```css
@keyframes slide {
  0% {
    left: 0;
    top: 0;
  }
  50% {
    left: 244px;
    top: 100px;
  }
  100% {
    left: 488px;
    top: 0;
  }
}
```

Once the keyframes for an animation have been declared they need to be assigned to an element.

```css
.stage:hover .ball {
  animation-name: slide;
}
```

`animation-duration` , `animation-name`, `animation-delay` and `animtion-timing-function` can also be set in the targeted element.
