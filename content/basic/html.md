# 目录
### html基础
<b><details><summary>1.HTML语义化</summary></b>
```
用正确的标签做正确的事情
根据内容的结构化（内容语义化），选择合适的标签（代码语义化）便于开发者阅读和写出更优雅的代码的同时让浏览器的爬虫和机器很好地解析
```
</details>

<b><details><summary>2.HTML语义化优点</summary></b>
```
1.为了在没有CSS的情况下，页面也能呈现出很好地内容结构、代码结构:为了裸奔时好看；  
2.用户体验：例如title、alt用于解释名词或解释图片信息、label标签的活用；  
3.有利于SEO：和搜索引擎建立良好沟通，有助于爬虫抓取更多的有效信息：爬虫依赖于标签来确定上下文和各个关键字的权重；
4.方便其他设备解析（如屏幕阅读器、盲人阅读器、移动设备）以意义的方式来渲染网页；
5.便于团队开发和维护，语义化更具可读性，是下一步吧网页的重要动向，遵循W3C标准的团队都遵循这个标准，可以减少差异化。
```
</details>

<b><details><summary>3.Doctype作用? 严格模式与混杂模式如何区分？它们有何意义?</summary></b>
```
（1）<!DOCTYPE>声明位于文档中的最前面的位置，处于标签之前。此标签可告知浏览器文档使用哪种 HTML 或 XHTML 规范。该标签可声明三种 DTD 类型，分别表示严格版本、过渡版本以及基于框架的HTML 文档

（2）所谓的标准模式是指，浏览器按 W3C 标准解析执行代码；
怪异模式则是使用浏览器自己的方式解析执行代码，因为不同浏览器解析执行的方式不一样，所以我们称之为怪异模式。 严格模式是浏览器根据web标准去解析页面，是一种要求严格的DTD，不允许使用任何表现层的语法，如严格模式的排版和JS 运作模式是以该浏览器支持的最高标准运行，混杂模式则是一种向后兼容的解析方法，说的透明点就是可以实现IE5.5以下版本浏览器的渲染模式
（3）浏览器解析时到底使用标准模式还是怪异模式，与你网页中的 DTD 声明直接相关， DTD 声明定义了标准文档的类型（标准模式解析）文档类型，会使浏览器使用相应的方式加载网页并显示，忽略 DTD 声明 ,将使网页进入怪异模式
```
</details>

<b><details><summary>4.HTML 与 XHTML 二者有什么区别，你觉得应该使用哪一个并说出理由。</summary></b>
```
应该使用XHTML，因为XHTML是XML重写了HTML的规范，比HTML更加严格，表现如下：
1、XHTML中所有的标记都必须有一个相应的结束标签；
2、XHTML所有标签的元素和属性的名字都必须使用小写；
3、所有的XML标记都必须合理嵌套；
4、所有的属性都必须用引号“”括起来；
5、把所有<和&特殊符号用编码表示；
6、给所有属性附一个值；
7、不要在注释内容中使用“--”；
8、图片必须使用说明文字。 
```
</details>

<b><details><summary>5.块级元素内联元素。</summary></b>
```
```
</details>

<b><details><summary>6.<script>在HTML文档中位置</summary></b>
```
https://www.jianshu.com/p/610743ddb6fe
```
</details>

<b><details><summary>7.HTML 本地存储</summary></b>
```
通过本地存储（Local Storage），web 应用程序能够在用户浏览器中对数据进行本地的存储。
在 HTML5 之前，应用程序数据只能存储在 cookie 中，包括每个服务器请求。本地存储则更安全，并且可在不影响网站性能的前提下将大量数据存储于本地。
与 cookie 不同，存储限制要大得多（至少5MB），并且信息不会被传输到服务器。
本地存储经由起源地（origin）（经由域和协议）。所有页面，从起源地，能够存储和访问相同的数据。
```
</details>

<b><details><summary>8.HTML5 应用程序缓存</summary></b>
```
使用应用程序缓存，通过创建 cache manifest 文件，可轻松创建 web 应用的离线版本。

HTML5 引入了应用程序缓存（Application Cache），这意味着可对 web 应用进行缓存，并可在没有因特网连接时进行访问。
应用程序缓存为应用带来三个优势：
离线浏览 - 用户可在应用离线时使用它们
速度 - 已缓存资源加载得更快
减少服务器负载 - 浏览器将只从服务器下载更新过或更改过的资源

更新缓存
一旦应用被缓存，它就会保持缓存直到发生下列情况：
用户清空浏览器缓存
manifest 文件被修改（参阅下面的提示）
由程序来更新应用缓存
```
</details>

<b><details><summary>9.XHTML 3中DTD</summary></b>
```
STRICT（严格类型）
TRANSITIONAL（过渡类型）
FRAMESET（框架类型）
```
</details>

<b><details><summary>10.表单提交中Get和Post方式的区别？</summary></b>
```
```
</details>




### HTML5

<b><details><summary>HTML5认识、优缺点?</summary></b>
```
HTML5 是最新的 HTML 标准。
HTML5 是专门为承载丰富的 web 内容而设计的，并且无需额外插件。
HTML5 拥有新的语义、图形以及多媒体元素。
HTML5 提供的新元素和新的 API 简化了 web 应用程序的搭建。
HTML5 是跨平台的，被设计为在不同类型的硬件（PC、平板、手机、电视机等等）之上运行。
优点：  
缺点：  
```
</details>

<b><details><summary>HTML5有哪些新特性、移除了哪些元素？</summary></b>
```  
新的语义/结构元素


新的表单元素
datalist
keygen
output

新的输入类型
color
date
datetime
datetime-local
email
month
number
range
search
tel
time
url
week

新的输入属性
autocomplete
autofocus
form
formaction
formenctype
formmethod
formnovalidate
formtarget
height 和 width
list
min 和 max
multiple
pattern (regexp)
placeholder
required
step

HTML5 - 新的属性语法

HTML5 图像

新的媒介元素


```
</details>

<b><details><summary>新的 HTML5 文档类型和字符集是？</summary></b>
```  
<!DOCTYPE html>
UTF-8
<meta charset="UTF-8" />
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
```
</details>  

<b><details><summary>HTML5 Canvas 元素有什么用？Canvas 与 SVG 的比较</summary></b>
```  
Canvas 元素用于在网页上绘制图形，该元素标签强大之处在于可以直接在 HTML 上进行图形操作

Canvas
依赖分辨率
不支持事件处理器
弱的文本渲染能力
能够以 .png 或 .jpg 格式保存结果图像
最适合图像密集型的游戏，其中的许多对象会被频繁重绘
SVG
不依赖分辨率
支持事件处理器
最适合带有大型渲染区域的应用程序（比如谷歌地图）
复杂度高会减慢渲染速度（任何过度使用 DOM 的应用都不快）
不适合游戏应用
```
</details>

<b><details><summary>HTML5媒体标签</summary></b>
```  
embed/audio/video
```
</details>

<b><details><summary>HTML5 废弃了哪些 HTML4 标签？</summary></b>
```  
```
</details>

<b><details><summary>HTML5 标准提供了哪些新的 API？</summary></b>
```  
```
</details>





### 浏览器

<b><details><summary>1.浏览器页面有哪三层构成，分别是什么，作用是什么?</summary></b>
```
构成：结构层、表示层、行为层   
分别是：HTML、CSS、JavaScript   
作用：HTML实现页面结构，CSS完成页面的表现与风格，JavaScript实现一些客户端的功能和业务。
```
</details>

<b><details><summary>你做的网页在哪些浏览器测试过,这些浏览器的内核分别是什么？</summary></b>
```  
a、 IE: trident 内核
b、 Firefox ： gecko 内核
c、 Safari:webkit 内核
d、 Opera: 以前是 presto 内核， Opera 现已改用 Google Chrome 的 Blink 内核
e、 Chrome:Blink( 基于 webkit ， Google 与 Opera Software 共同开发 )
```
</details>
