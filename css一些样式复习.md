- -webkit-text-size-adjust 的本职是用于mobile的 
1. 采用-webkit-text-size-adjust: 100%;
2. 必须要用小于12px字体时，用-webkit-transform: scale( )缩小到合适值。
参考 [关于text-size-adjust] (http://www.jianshu.com/p/9fad261dd3e1 , 关于text-size-adjust)
- vertical-align详解
参考 [vertical-align详解] (http://www.cnblogs.com/hykun/p/3937852.html , 这篇写得超级好~~)

- rem（root em，根em）：是CSS3新增的一个相对单位，这个单位引起了广泛关注。这个单位与em有什么区别呢？区别在于使用rem为元素设定字体大小时，仍然是相对大小，但相对的只是HTML根元素。这个单位可谓集相对大小和绝对大小的优点于一身，通过它既可以做到只修改根元素就成比例地调整所有字体大小，又可以避免字体大小逐层复合的连锁反应。目前，除了IE8及更早版本外，所有浏览器均已支持rem。对于不支持它的浏览器，应对方法也很简单，就是多写一个绝对单位的声明。这些浏览器会忽略用rem设定的字体大小。
- 处理 Chrome 与其它浏览器中关于 'outline' 的不一致性。
```
a:focus {
outline: thin dotted;
}
```
- [normalize.css]  (http://colorski.com/l/l-h/7.html , 关于浏览器的差异~记记记)
