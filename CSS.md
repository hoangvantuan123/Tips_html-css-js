# Awesome CSS Tips

#### Contents

- [Cursors](#cursors)
- [Scroll Snap](#Scroll-Snap)
- [Responsive Flex Wrap](#Responsive-Flex-Wrap)
- [Grid-repeat-auto-minmax](#Grid-repeat-auto-minmax)

## Cursors

Tùy chọn thay đổi cursors có thể sử dụng hình ảnh của riêng bạn , hoặc thậm chí là biểu tượng cảm xúc.

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


## Responsive Flex Wrap

```css
.container{
    display:flex;
    flex-wrap:wrap;
}
.item{

   flex: 1 1 150px;
   /*
   1: flex-grow
   1: flex-Shrink
   150px: flex-basis
   */
}
```

## Grid repeat-auto-minmax

Lưới trong CSS tự động
```css
.grid {
    display:grid;
    grid-template-columns: repeat(auto-fit ,minmax(150px,1fr));
}

```


