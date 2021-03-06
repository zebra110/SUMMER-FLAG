记录一个tip~webstorm 格式化代码的快键键Ctrl+Alt+l.

- display常见的例子是：把 li 元素修改成 inline，制作成水平菜单/给内联元素设置高度
- 使用 max-width 替代 width 可以使浏览器更好地处理小窗口的情况
- 当你设置一个元素为 box-sizing: border-box; 时，此元素的内边距和边框不再会增加它的宽度
- absolute 是最棘手的position值。 absolute 与 fixed 的表现类似，但是它不是相对于视窗而是相对于最近的“positioned”祖先元素。
- 记住一个“positioned”元素是指 position 值不是 static 的元素。
- 解决图片一出盒子~

```stylus
  .clearfix {
    overflow: auto;
    zoom: 1;
  }
```

- 使用 Flexbox 的居中布局

```stylus
.vertical-container {
  height: 300px;
  display: -webkit-flex;
  display:         flex;
  -webkit-align-items: center;
          align-items: center;
  -webkit-justify-content: center;
          justify-content: center;
}
```
- 媒体查询

```stylus
@media screen and (min-width:600px) {
  nav {
    float: left;
    width: 25%;
  }
  section {
    margin-left: 25%;
  }
}
@media screen and (max-width:599px) {
  nav li {
    display: inline;
  }
}
```

- 用 display 属性的值 inline-block 来实现float:left的效果 重点是不用清除浮动了~超酷 但是要注意、、
 1. vertical-align 属性会影响到 inline-block 元素，你可能会把它的值设置为 top 。
 2. 你需要设置每一列的宽度
 3. 如果HTML源代码中元素之间有空格，那么列与列之间会产生空隙
 
- 轻松的实现文字的多列布局两种方法
1. 

```stylus
.bottom-nav dl {
    float: left;
    width: 18.5%;
}
```

2.

```stylus
.three-column {
  padding: 1em;
  -moz-column-count: 3;
  -moz-column-gap: 1em;
  -webkit-column-count: 3;
  -webkit-column-gap: 1em;
  column-count: 3;
  column-gap: 1em;
}
```

- 使用 Flexbox 的布局

```stylus
.container {
  display: -webkit-flex;
  display: flex;
}
.initial {
  -webkit-flex: initial;
          flex: initial;
  width: 200px;
  min-width: 100px;
}
.none {
  -webkit-flex: none;
          flex: none;
  width: 200px;
}
.flex1 {
  -webkit-flex: 1;
          flex: 1;
}
.flex2 {
  -webkit-flex: 2;
          flex: 2;
}
```
- 使用 Flexbox 的居中布局(CSS里总算是有了一种简单的垂直居中布局的方法了！)

```stylus
.vertical-container {
  height: 300px;
  display: -webkit-flex;
  display:         flex;
  -webkit-align-items: center;
          align-items: center;
  -webkit-justify-content: center;
          justify-content: center;
}
```
