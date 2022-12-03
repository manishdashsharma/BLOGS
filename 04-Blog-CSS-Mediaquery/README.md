### CSS-Media Query

Media queries are basically a way to write conditional CSS. That means CSS markup that the browser will only render if certain conditions are met. Its most commonly use is in responsive design, where it’s a way to tell browsers to change the display of website elements when above or below a certain screen size. However, as we will see below, there are other ways you can use them.

### How Do You Write a Media Query?

So, what is the correct way to use a media query? In CSS, they part of the at-rules, in this case `@media`. You then add the type of media you are trying to target and the feature/condition that needs to be met for the query to take effect.

```css
@media [media-type] ([media-feature]) {
	// custom CSS
}
```
For example, the code snippet below targets devices with screens above 320 pixels. Everything that’s placed inside curly brackets of the media query will only be output in the browser on devices with screens that meet that condition. This is also called a break point, meaning a point at which the design changes notably to accommodate a different screen size.

```css
@media screen and (min-width: 320px) {
	// custom CSS
}
```
### Operators in Media Queries

In CSS media queries, you can also use operators like and, or, and not to combine conditions like so:

```css
@media screen and (min-width: 320px) and (max-width: 786px) {
	// custom CSS
```

In the above example we have amended the original query to not only have a minimum screen size at which it will go into effect but also a maximum at which it will no longer apply. There’s also only, which makes a style apply only if the entire query matches. It is also often used to improve compatibility of media queries with older browsers. 

### Available Media Types
While `screen` is the most common type of media to query, we have other options:
- `all` — Targets all devices
- `print` — For documents that are viewed in print preview or media that displays content in a way that is intended for print
- `speech` — Devices that read out content like screen readers

### Examples for Media Features/Conditions

In the context of media queries for responsive design, the most common media feature is width, including min-width and max-width. However, you also have more choices here, such as:
- `height` — Pretty much the same as width but for device height. Also takes min-height and max-height to define ranges.
- `aspect-ratio` — Targets the width-to-height ration of the viewport.
- `orientation` — Lets you apply queries depending on whether a device is in portrait or landscape mode.
- `hover` — Introduce conditional CSS for devices that have different ways of hovering over elements, like a mouse vs a touchscreen.

<iframe height="300" style="width: 100%;" scrolling="no" title="media" src="https://codepen.io/manishdashsharma/embed/poKLmpB?default-tab=html%2Cresult&editable=true&theme-id=dark" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/manishdashsharma/pen/poKLmpB">
  media</a> by Manish Dash Sharma (<a href="https://codepen.io/manishdashsharma">@manishdashsharma</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

**There are some common breakpoints, not a standard resolution, that can be used for the different widths & heights of devices:**

- For Mobile devices `320px-480px`
- For Tablets or iPad `480px - 768px`
- For Laptop or small-size screen `768px -1024px`
- For Desktop or large-size screen `1024px -1200px`
- For Extra-large size device `1200px` 

### Thank you !

We have discussed media-quer , obviously it has more to it . I hope you have found this article useful. If so, be sure to share and comment !

