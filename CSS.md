# Awesome CSS Tips

#### Contents

- [Cursors](#cursors)
- [Scroll Snap](#scrollsnap)

## Cursors

Did you know that you can use your own image, or even emoji as a cursor?

```css
div {
    cursor: url('path-to-image.png'), url('path-to-fallback-image.png'), auto;
}
```

[Link to Codepen](https://codepen.io/denic/pen/bGVpOPj)

## scrollsnap

```css

.container {
    display:flex;
    overflow:auto;
    scroll-snap-type:x mandatory;
}
.container> .item {

    min-width:100%;
    scroll-snap-align:start;
}
```
