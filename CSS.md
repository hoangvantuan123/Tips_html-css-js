# Awesome CSS Tips

#### Contents

- [Reponsive Screen Sizes](#Responsive-Screen-Sizes)
- [Cursors](#cursors)
- [Scroll Snap](#Scroll-Snap)
- [Responsive Flex Wrap](#Responsive-Flex-Wrap)
- [Grid-repeat-auto-minmax](#Grid-repeat-auto-minmax)
- [Drop Caps](#Drop-Caps)





## Responsive Screen Sizes
Một thành phần chính trong thiết kế đáp ứng tạo ra một trải nghiệm phù hợp.

```css
/*Mobile*/
@media only screen and (max-width: 600px) {

}

/* Tablet */
@media only screen and (max-width: 768px) {

}

/* Laptop */
@media only screen and (max-width: 992px) {

}

/* Large Screen */
@media only screen and (max-width: 1200px) {

}
```
Bạn viết tham khảo :

[Link](https://css-tricks.com/snippets/css/media-queries-for-standard-devices/)

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

## Drop-Caps

Chữ to ở đầu dòng
```css
.text::first-letter{
   font-size: 3rem;
   float: left;
   margin-right:10px;
}
```




