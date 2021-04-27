### 1.如何强制页面加载JavaScript中的其他页面

![image-20210427141337671](C:\Users\Administrator\AppData\Roaming\Typora\typora-user-images\image-20210427141337671.png)

### 2.escape字符是用来做什么的

使用特殊字符（如单引号，双引号，撇号和＆符号）时，将使用转义字符（反斜杠）。在字符前放置反斜杠，使其显示。

### 3.什么是JavaScript Cookie

Cookie是用来存储计算机中的小型测试文件，当用户访问网站以存储他们需要的信息时，它将被创建。

### 4.使用innerHTML的缺点

1. 内容随处可见；不能像“追加到innerHTML”一样使用；
2. 即使你使用+ = like“innerHTML = innerHTML +'html'”旧的内容仍然会被html替换；
3. 整个innerHTML内容被重新解析并构建成元素，因此它的速度要慢得多；
4. innerHTML不提供验证，因此我们可能会在文档中插入有效的和破坏性的HTML并将其中断。

### 5.break和continue语句的作用

- Break语句从当前循环中退出。
- continue语句继续下一个循环语句。

### 6.在JavaScript中，dataypes的两个基本组是什么

- Primitive
- Reference types

### 7.哪些关键字用于处理异常

try... Catch-finally用于处理JavaScript中的异常。

### 8.JavaScript中不同类型的错误有几种

- Load time errors：该错误发生于加载网页时，例如出现语法错误等状况，称为加载时间错误，并且会动态生成错误。
- Run time errors：由于在HTML语言中滥用命令而导致的错误。
- Logical Errors：这是由于在具有不同操作的函数上执行了错误逻辑而发生的错误。

### 9.获得CheckBox状态的方式

alert（document.getElementById（'checkbox1'）。checked）;

如果CheckBox被检查，此警报将返回TRUE。

### 10.window.onload和onDocumentReady

- 在载入页面的所有信息之前，不运行onload函数。这导致在执行任何代码之前会出现延迟。
- onDocumentReady在加载DOM之后加载代码。这允许早期的代码操纵。

