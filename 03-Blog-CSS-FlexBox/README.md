### CSS-flexBox : 
CSS Flexbox is a CSS property to align and organize the elements inside a container efficiently. A CSS Flexbox starts by creating a flexible space on the web page called a container (the outer layer) that can expand as we insert various elements into it, called items. The expansion also includes the spacing that each item would take to fill the space in the container. The Flexbox in CSS grows in the direction of a single axis which can be either horizontal or vertical .

### Flexbox comprises two elements :
1. a container 
2. an item(s)

The container is the outside layer, while the items are the elements encapsulated in it . In easy term we can say a container is the parent and the item(s) are the child of that parent .

### display

This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children. Once we have attached the `display: flex` property to a container, everything inside the container will work according to the flex properties.

```css
.container {
display: flex;
}
```
### flex-direction

The flex-direction property takes the following values:
- `row`: This is the default arrangement. If the writing mode is ltr then the row will arrange the items in the left to the right direction or else right to left.
- `row-reverse`: This is the reverse of what the value row would have produced in both writing modes.
- `column`: Column value will make the main axis vertical, and the items will be arranged from top to bottom with this value.
- `column-reverse`: This is the reverse of what the value column would have produced.

```css
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```
<iframe height="500" style="width: 100%;" scrolling="no" title="flex-direction" src="https://codepen.io/manishdashsharma/embed/YzvaWom?default-tab=html%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/manishdashsharma/pen/YzvaWom">
  flex-direction</a> by Manish Dash Sharma (<a href="https://codepen.io/manishdashsharma">@manishdashsharma</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

## flex-warp

Like the word-wrap property, the flex-wrap property seeks to wrap the items inside the container to the next line in case of insufficient space. By default, the items do not wrap and are arranged in a single line along the main axis—the flex-wrap works from top to bottom.

The flex-wrap property takes on the following values:

- `nowrap`: The items will be arranged in a single line. It is the default value of flex-wrap and can lead to the overflow of the flex container.
- `wrap`: Wrap the items to the next line when required.
- `wrap-reverse`: Wrap the items to the next line when needed but in the reverse order.

```css
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```
<iframe height="300" style="width: 100%;" scrolling="no" title="flex-warp" src="https://codepen.io/manishdashsharma/embed/WNyzOVR?default-tab=html%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/manishdashsharma/pen/WNyzOVR">
  flex-warp</a> by Manish Dash Sharma (<a href="https://codepen.io/manishdashsharma">@manishdashsharma</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

### justify-content

The justify-content property aligns the elements along the main axis and distributes the leftover space equally within these items.

The justify-content property in CSS Flexbox takes the following values:

- `flex-start`: The Flexbox items are arranged towards the start of the axis.
- `flex-end`: The items of Flexbox in CSS are arranged towards the end of the axis.
- `start`: The items are arranged toward the start of the writing mode direction.
- `end`: The items are arranged towards the end of the writing mode direction.
center: The items are packed along the center of the container (or main axis).
- `space-between`: The items are spaced equally on the line, with the first item at the start of the line and the last item at the end of the line.
- `space-around`: The items have an equal amount of space around them. With this value, the first item does not touch the container as in space-between. The same rule applies to the last item.
- `space-evenly`: The items are packed with equal space all around them. The difference between space-around and space-evenly is that in space-around, the edge space is x in the start item while the right space is 2x. It is because the next item will also have a space of x around it.

```css
.container {
  justify-content: flex-start | flex-end | 
  center | space-between | space-around | 
  space-evenly | start | end | left | right ;
}
```
<iframe height="300" style="width: 100%;" scrolling="no" title="flex-justify content" src="https://codepen.io/manishdashsharma/embed/OJEvjgW?default-tab=html%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/manishdashsharma/pen/OJEvjgW">
  flex-justify content</a> by Manish Dash Sharma (<a href="https://codepen.io/manishdashsharma">@manishdashsharma</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

### align-items

This defines the default behavior for how flex items are laid out along the cross axis on the current line. Think of it as the justify-content version for the cross-axis (perpendicular to the main-axis).

```css
.container {
  align-items: stretch | flex-start | flex-end | 
  center | baseline | first baseline | last baseline | 
  start | end |self-start | self-end ;
}
```
- `flex-start`: The cross-start margin edge of the flex item is placed flush with the cross-start edge of the line.
- `flex-end`: The cross-end margin edge of the flex item is placed flush with the cross-end edge of the line.
- `center`: The flex item’s margin box is centered in the cross axis within the line. (If the cross size of the flex line is less than that of the flex item, it will overflow equally in both directions.)
<iframe height="300" style="width: 100%;" scrolling="no" title="align-items" src="https://codepen.io/manishdashsharma/embed/ExREbZw?default-tab=html%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/manishdashsharma/pen/ExREbZw">
  align-items</a> by Manish Dash Sharma (<a href="https://codepen.io/manishdashsharma">@manishdashsharma</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

### order

The appearance of the Flexbox items is fixed according to how they are written inside the HTML source code. So an element (say A) written before another element (say B) will appear ahead of B in the Flexbox container. This order, however, can be altered with the “order” property of the Flexbox items. The order property takes an integer value and arranges the elements from lower to higher order (lower number means high priority). You can also consider this arrangement in ascending order.
```css
.item {
  order: 5; /* default is 0 */
}
```

<iframe height="300" style="width: 100%;" scrolling="no" title="order" src="https://codepen.io/manishdashsharma/embed/BaVrmmB?default-tab=html%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/manishdashsharma/pen/BaVrmmB">
  order</a> by Manish Dash Sharma (<a href="https://codepen.io/manishdashsharma">@manishdashsharma</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

### align-self

This allows the default alignment (or the one specified by align-items) to be overridden for individual flex items.

```css
.item {
  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}
```
### the flex property

The flex property defines three different sets of values. The first one is for `flex-grow`, the second one for `flex-shrink`, and the last one for `flex-basis`. So, the syntax would follow the following structure:

```css
.item {
  flex-grow: 4; /* default 0 */
}
```
```css
.item {
  flex-shrink: 3; /* default 1 */
}
```
```css
.item {
  flex-basis:  | auto; /* default auto */
}
```
### Conclusion

We have discussed a lot about flex , obviously it has more to it . I hope you have found this article useful. If so, be sure to share and comment !
