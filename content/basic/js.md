# js

<b><details><summary>1.暂时性死区</summary></b>
```
在代码块内，使用let命令声明变量之前，该变量都是不可用的。这在语法上，称为“暂时性死区”（temporal dead zone，简称TDZ）

只要块级作用域内存在let命令，它所声明的变量就“绑定”（binding）这个区域，不再受外部的影响。

https://www.cnblogs.com/ricoliu/p/6149912.html
```
</details>