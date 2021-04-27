### 1.ViewState和SessionState有什么区别

- “ViewState”特定于会话中的页面。
- “SessionState”特定于可在Web应用程序中的所有页面上访问的用户特定数据。

2.如何使用JavaScript提交表单

`document.form [0] .submit（）`

### 3.元素的样式/类如何改变

1. `document.getElementById(“myText”).style.fontSize = “20?;`
2. `document.getElementById(“myText”).className = “anyclass”;`

### 4.JavaScript中的循环结构都有什么

For、While、do-while loops

### 5.如何将base字符串转换为integer

1. parseInt() 函数解析一个字符串参数，并返回一个指定基数的整数。
2. parseInt（）将要转换的字符串作为其第一个参数，第二个参数是给定字符串的基础。
3. 为了将4F（基数16）转换为整数，所使用的代码是 ：`parseInt ("4F", 16);`

### 6.如何检测客户端机器上的操作系统

使用navigator.appVersion字符串（属性）。

### 7.NULL是什么意思

NULL用于表示无值或无对象。它意味着没有对象或空字符串，没有有效的布尔值，没有数值和数组对象。

### 8.delete操作符的功能是什么

- 用于删除程序中的所有变量或对象。
- 不能删除使用VAR关键字声明的变量。

### 9.JavaScript中有哪些类型的弹出框

Alert、Confirm and、Prompt

### 10.Void（0）怎么用

- Void（0）用于防止页面刷新，并在调用时传递参数“zero”。
- Void（0）用于调用另一种方法而不刷新页面。