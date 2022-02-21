# Awesome CSS Tips

#### Contents

- [Cursors](#cursors)
- [Scroll Snap](#Scroll-Snap)

## Cursors

Tùy chọn thay đổi cursors có thể sử dụng hình ảnh của riêng bạn , hoặc thậm

```css
div {
    cursor: url('path-to-image.png'), url('path-to-fallback-image.png'), auto;
}
```

[Link to Codepen](https://codepen.io/denic/pen/bGVpOPj)

## Scroll Snap
Scroll Snap là một thuộc tính CSS giúp tạo băng chuyền như ví dụ sau :
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
