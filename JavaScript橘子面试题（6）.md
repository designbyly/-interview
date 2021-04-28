## 1.ECMAScript和JavaScript的关系

前者是后者的规格，后者是前者的一种实现（另外的ECMAScript方言还有Jscript和ActionScript）。日常场合，这两个词是可以互换的。

## 2.ES6与ECMAScript 2015的关系

1. ES6既是一个历史名词，也是一个泛指，含义是5.1版以后的JavaScript的下一代标准，涵盖了ES2015、ES2016、ES2017等等。
2. ES2015则是正式名称，特指该年发布的正式版本的语言标准。

## 3.语法提案的批准流程

- Stage 0 - Strawman（展示阶段）
- Stage 1 - Proposal（征求意见阶段）
- Stage 2 - Draft（草案阶段）
- Stage 3 - Candidate（候选人阶段）
- Stage 4 - Finished（定案阶段）

## 4.说一下Babel转码器

[Babel](https://babeljs.io/)是一个广泛使用的ES6转码器，可以将ES6代码转为ES5代码，从而在现有环境执行。

## 5.了解Traceur转码器吗

Google公司的[Traceur](https://github.com/google/traceur-compiler)转码器，也可以将ES6代码转为ES5代码。

## 6.Traceur是否可以在线转换，使用过没

Traceur也提供一个[在线编译器](http://google.github.io/traceur-compiler/demo/repl.html)，可以在线将ES6代码转为ES5代码。转换后的代码，可以直接作为ES5代码插入网页运行。

## 7.解释数组的解构赋值

1. ES6允许按照一定模式，从数组和对象中提取值，对变量进行赋值，这被称为解构（Destructuring）。

2. 以前，为变量赋值，只能直接指定值。

3. ```javascript
   var [a, b, c] = [1, 2, 3];
   ```

### 8.不完全解构和默认值情况

略，太多，橘子写不过来

## 9.字符串的解构赋值

字符串被转换成了一个类似数组的对象。

```javascript
const [a, b, c, d, e] = 'hello';
a // "h"
b // "e"
c // "l"
d // "l"
e // "o"
let {length : len} = 'hello';
len // 5
```

## 10.解构赋值的规则是

只要等号右边的值不是对象，就先将其转为对象。由于`undefined`和`null`无法转为对象，所以对它们进行解构赋值，都会报错。