### What is CSS-position property ?
The CSS position property is used to specify where an element is displayed on the page. When paired with the the top, right, bottom, and left CSS properties, the position property determines the final location of the element.

### what are the position property ?
1. static
2. relative
3. fixed
4. absolute
5. sticky

### Let’s break down each value in detail with examples to see how each value affects a page element :

- **position: static**
`position: static` , the default position for HTML elements. Elements are positioned based on the normal flow of the page, as you would expect them to be without any CSS styling. They are not affected by the top, right, bottom, or left properties. 
<iframe height="300" style="width: 100%;" scrolling="no" title="static" src="https://codepen.io/manishdashsharma/embed/poKaBBq?default-tab=html%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/manishdashsharma/pen/poKaBBq">
  static</a> by Manish Dash Sharma (<a href="https://codepen.io/manishdashsharma">@manishdashsharma</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

- **position : relative**
`position: relative`, an element follows the render flow of the page, but will be shifted relative to its initial position . To determine , you must set values for the top, right, bottom, and/or left properties. Other elements won’t be affected . Z-Index which will help you to bring something front.
  <iframe height="300" style="width: 100%;" scrolling="no" title="relative" src="https://codepen.io/manishdashsharma/embed/LYrQoRx?default-tab=html%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/manishdashsharma/pen/LYrQoRx">
  relative</a> by Manish Dash Sharma (<a href="https://codepen.io/manishdashsharma">@manishdashsharma</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

- **position : fixed**
`position: fixed` ,element doesn't follow the normal render flow of the document . Fixed elements do not move when the user scrolls . You can use the top, right, bottom, and left properties to set the fixed element's final position.
<iframe height="300" style="width: 100%;" scrolling="no" title="fixed" src="https://codepen.io/manishdashsharma/embed/bGKLyRO?default-tab=html%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/manishdashsharma/pen/bGKLyRO">
  fixed</a> by Manish Dash Sharma (<a href="https://codepen.io/manishdashsharma">@manishdashsharma</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

- **position : absolute**
`absolute property`, will completely remove the element from the the document.You can position this element anywhere with respect to its parent. Its final position is determined by the values of top, right, bottom, and left.
<iframe height="300" style="width: 100%;" scrolling="no" title="absolute" src="https://codepen.io/manishdashsharma/embed/wvXybxO?default-tab=html%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/manishdashsharma/pen/wvXybxO">
  absolute</a> by Manish Dash Sharma (<a href="https://codepen.io/manishdashsharma">@manishdashsharma</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

- **position : sticky**
This sticky property is to fix something until the page scrolls to a point where the element hits the top, left, right, or bottom value specified. It is fixed in a spot and appears to “stick” to the page as the user scrolls.
<iframe height="300" style="width: 100%;" scrolling="no" title="sticky" src="https://codepen.io/manishdashsharma/embed/YzvebBL?default-tab=html%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/manishdashsharma/pen/YzvebBL">
  sticky</a> by Manish Dash Sharma (<a href="https://codepen.io/manishdashsharma">@manishdashsharma</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

###Conclusion
We have discussed positioning in CSS which includes:
1. `position: static`
2. `position :fixed`
3. `position :relative`
4. `position :absolute`
5. `position :sticky`

**I hope you have found this article useful. If so, be sure to share and comment !**