# CSS Review of Transforms Transitions and Animations

I think this is one of my favorite uses of CSS. It can be tricky but when it is done well it can really make an app or site fun to interact with.

Transitions allow the developer to manipulate the scale of an element. For example, take a playing card, it is possible allow an element to flip on screen giving it a life like style and appreciation. By using `transform` you can rotate an element. There are other factors that help animate this too. `@keyframes` and `animation` add to the overall affect. `Scale` is also another important value to be aware of. This allows you to make the element larger or smaller.

This article goes over the use of these and provides excellent examples to help you implement them in your next project. One of my favorite that I used in a project recently was the Multiple Scaling Demo. I implemented something similar for a card flip memory game. It was fun and not too difficult.

```css

.box-1 {
  transform: scaleX(.5);
}
.box-2 {
  transform: scaleY(1.15);
}
.box-3 {
  transform: scale(.5, 1.15);
}

```
Transitions are used on elements in order to change a state of that element. Common states are, `:hover, :focus, :active`, and `:target pseudo-classes`. Transitions can change movement and color on screen. By paring this with `transitional property`, you can manipulate the properties in conjunction with other transitional properties. You can take a square box and turn it into a circle!

Some of these transitional properties to consider are:

background-color
background-position
border-color
border-width
border-spacing
bottom
clip
color
crop
font-size
font-weight
height
left
letter-spacing
line-height
margin
max-height
max-width
min-height
min-width
opacity
outline-color
outline-offset
outline-width
padding
right
text-indent
text-shadow
top
vertical-align
visibility
width
word-spacing

You can specify the duration of the transitions using `transition-duration` too. The tutorial goes in depth and shows you how to implement many of the fun animations and transitions.

Finally, `Web Designer Depot`, discusses eight simple ways to include simple effects that will excite and engage your users. The article provided examples and code that can be easily included in upcoming projects.

1. Fade In
2. Change Color
3. Grow and Shrink
4. Rotate Elements
5. Square to Circle
6. 3D shadow
7. Swing
8. Inset Border

Finally, many of the above transitions and animations can be applied to buttons, text, and create fun little animations. As I work on my CSS I will try to find ways to include some of these tricks.
