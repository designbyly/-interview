### 1.说一说你对js函数的认识

- 函数是一等公民
- 函数可以有属性，并且能连接到它的构造方法
- 函数可以像一个变量一样存在内存中
- 函数可以当做参数传给其他函数
- 函数可以返回其他函数

### 2.如何创建数组,

```
var myArray = [];
```

### 3.JavaScript 中的提升操作

提升（hoisting）是 JavaScript 解释器将所有变量和函数声明移动到当前作用域顶部的操作。有两种类型的提升：

- 变量提升——非常少见
- 函数提升——常见

### 4.说明Revealing Module Pattern 设计模式

暴露模块模式（Revealing Module Pattern）是模块模式的一个变体，目的是维护封装性并暴露在对象中返回的某些变量和方法。缺点是无法引用私有方法。

### 5.什么是JavaScript？

JavaScript是客户端和服务器端脚本语言，可以插入到HTML页面中，并且是目前较热门的Web开发语言。同时，JavaScript也是面向对象编程语言。

### 6.JavaScript和ASP脚本相比，哪个更快？

- JavaScript更快。JavaScript是一种客户端语言，因此它不需要Web服务器的协助来执行。
- 另一方面，ASP是服务器端语言，因此总是比JavaScript慢。值得注意的是，Javascript现在也可用于服务器端语言（nodejs）。

### 7.什么是负无穷大

负无穷大是JavaScript中的一个数字，可以通过将负数除以零来得到。

### 8.如何将JavaScript代码分解成几行

- 在字符串语句中可以通过在第一行末尾使用反斜杠“\”来完成
- 如果不是在字符串语句中更改为新行，那么javaScript会忽略行中的断点。

### 9.什么是未声明和未定义的变量

1. 未声明的变量：是程序中不存在且未声明的变量，如果程序尝试读取未声明变量的值，则会遇到运行时错误。
2. 未定义的变量：是程序中声明但尚未给出任何值的变量，如果程序尝试读取未定义变量的值，则返回未定义的值。

### 10.如何编写可动态添加新元素的代码

![image-20210427140429597](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210427140429597.png)

