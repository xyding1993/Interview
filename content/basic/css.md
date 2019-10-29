# 目录 css

<b><details><summary>1.CSS盒模型。</summary></b>
```
盒子模型简单点理解就是外边距(margin)+边框(border)+内边距(padding)+内容(content)，页面所呈现的效果其实就是一个个盒子堆叠而成的
有两种，W3C盒子模型(标准盒模型)和IE盒子模型(怪异盒模型)
```
</details>

<b><details><summary>2.标准模型+IE模型</summary></b>
```
在标准模式下的盒模型，盒子实际内容（content）的width/height=我们设置的width/height;盒子总宽度/高度=width/height+padding+border+margin  
在怪异模式下的盒模型，盒子实际内容（content）的width/height+内边距padding+边框border宽度=我们设置的width/height，盒子总宽度/高度=width/height + margin = 内容区宽度/高度 + padding + border + margin
```
</details>

<b><details><summary>3.CSS如何指定盒子模型的种类</summary></b>
```
box-sizing 属性允许以特定的方式定义匹配某个区域的特定元素。
content-box(W3C（标准盒模型）)
border-box(IE盒子模型（怪异盒模型）)
inherit
```
</details>

<b><details><summary>4.JS如何获取盒模型的高宽</summary></b>
```
1.dom.style.width/height   
这种方法只能获取使用内联样式的元素的宽和高。 
也就是说如果该节点的样式是在style标签中或是外部的CSS样式表中的话，通过这种方法是没办法获取dom的宽高的。 
2.dom.currentStyle.width/height   
这种方法获取的是浏览器渲染以后的元素的宽和高，无论是用何种方式引入的css样式都可以，但只有IE浏览器支持这种写法。  
无论以哪种方式，内联也好，style标签中也好，都可以获取的到。但是这种方法只能在IE浏览器中使用
3.window.getComputedStyle(dom).width/height   
这种方法获取的也是浏览器渲染以后的元素的宽和高，但这种写法兼容性更好一些。  
4.dom.getBoundingClientRect().width/height  
这种方法经常使用的场所是，计算一个元素的绝对位置（相对于视窗左上角），它能拿到元素的left、top、width、height 4个属性。
```
</details>

<b><details><summary>5.根据盒模型解释边距重叠</summary></b>
```
边界重叠是指两个或多个盒子(可能相邻也可能嵌套)的相邻边界(其间没有任何非空内容、补白、边框)重合在一起而形成一个单一边界。
两个或多个块级盒子的垂直相邻边界会重合，它们的边界宽度是相邻边界宽度中的最大值。注意水平边界是不会重合的
```
</details>

<b><details><summary>6.BFC</summary></b>
```
概念：块级格式化上下文

BFC的原理（BFC的渲染规则）：
在BFC这个元素垂直方向的边距会发生重叠；
BC的区域不会与浮动元素的box重叠（用来清除浮动和做布局）；
BC在页面上是一个独立的容器，其里外的元素不会互相影响；
计算BFC高度的时候，浮动元素也会参与计算；

创建BFC的方法:
1.float值不为none
2.position值不为static和absolute
3.display属性为table/table-cell等与table相关的值
4.overflow值不为visible

BFC的使用场景：
1.BFC垂直方向边距重叠的问题；
2.BFC不与float重叠；
3.清除浮动
```
</details>

<b><details><summary>7.隐藏元素的几种方式</summary></b>
```
visiblity visiblity:hidden
display display:none
opacity opacity:0
position position: absolute;left: -200px;
```
</details>

<b><details><summary>8.伪元素伪类</summary></b>
```
伪元素使用2个冒号，常见的有：::before，::after，::first-line，::first-letter，::selection、::placeholder等；
伪类使用1个冒号，常见的有：:hover，:link，:active，:target，:not()，:focus等

区别：
伪元素添加了一个页面中没有的元素（只是从视觉效果上添加了，不是在文档树中添加），伪类是给页面中已经存在的元素添加一个类。

CSS3中的伪元素
CSS2 中的伪元素使用1个冒号，在 CSS3 中，为了区分伪类和伪元素，规定伪元素使用2个冒号。
如果不需要考虑IE8以下的浏览器，建议都使用2个冒号的新标准写法来写。否则还是使用1个冒号。

```
</details>