# Awesome CSS Tips

#### Contents

- [Cursors](#cursors)
- [Scroll Snap](#scroll_snap)

## Cursors

Did you know that you can use your own image, or even emoji as a cursor?

```css
div {
    cursor: url('path-to-image.png'), url('path-to-fallback-image.png'), auto;
}
```

[Link to Codepen](https://codepen.io/denic/pen/bGVpOPj)

## scroll_snap

```css

.container {
    display:flex
}
