# 目录 css

<b><details><summary>1.CSS盒模型。</summary></b>
```
盒子模型简单点理解就是外边距(margin)+边框(border)+内边距(padding)+内容(content)，页面所呈现的效果其实就是一个个盒子堆叠而成的
有两种，W3C盒子模型(标准盒模型)和IE盒子模型(怪异盒模型)
```
</details>

<b><details><summary>2.标准模型+IE模型</summary></b>
在标准模式下的盒模型，盒子实际内容（content）的width/height=我们设置的width/height;盒子总宽度/高度=width/height+padding+border+margin  
在怪异模式下的盒模型，盒子实际内容（content）的width/height+内边距padding+边框border宽度=我们设置的width/height，盒子总宽度/高度=width/height + margin = 内容区宽度/高度 + padding + border + margin
```
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
```
</details>

<b><details><summary>5.根据盒模型解释边距重叠</summary></b>
```
```
</details>

<b><details><summary>6.BFC</summary></b>
```
```
</details>