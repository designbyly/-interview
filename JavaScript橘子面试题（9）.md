## 1.ES6提供二进制和八进制数值的新的写法

前缀`0b`（或`0B`）和`0o`（或`0O`）表示。

## 2.ES6在Number对象上，提供了啥新方法

新提供了`Number.isFinite()`和`Number.isNaN()`两个方法。

### 3.ES6三角函数方法有哪些

- `Math.sinh(x)` 返回`x`的双曲正弦（hyperbolic sine）
- `Math.cosh(x)` 返回`x`的双曲余弦（hyperbolic cosine）
- `Math.tanh(x)` 返回`x`的双曲正切（hyperbolic tangent）
- `Math.asinh(x)` 返回`x`的反双曲正弦（inverse hyperbolic sine）
- `Math.acosh(x)` 返回`x`的反双曲余弦（inverse hyperbolic cosine）
- `Math.atanh(x)` 返回`x`的反双曲正切（inverse hyperbolic tangent）

## 4.说一下指数运算符写法

ES7新增了一个指数运算符（`**`），目前Babel转码器已经支持。

## 5.ES6提供三个新的遍历数组的方法

`entries()`，`keys()`和`values()

## 6.ES5对空位的处理

- `forEach()`, `filter()`, `every()` 和`some()`都会跳过空位。
- `map()`会跳过空位，但会保留这个值
- `join()`和`toString()`会将空位视为`undefined`，而`undefined`和`null`会被处理成空字符串。

## 7.rest参数听说过吗

- （形式为“...变量名”），用于获取函数的多余参数，这样就不需要使用arguments对象了。
- rest参数搭配的变量是一个数组，该变量将多余的参数放入数组中。

## 8.说一下严格模式

从ES5开始，函数内部可以设定为严格模式。

```javascript
function doSomething(a, b) {
  'use strict';
  // code
}
```

## 9.尾递归优化的实现

尾递归优化只在严格模式下生效，那么正常模式下，或者那些不支持该功能的环境中，有没有办法也使用尾递归优化呢？回答是可以的，就是自己实现尾递归优化。

只要减少调用栈，就不会溢出。采用“循环”换掉“递归”。

下面是一个正常的递归函数。

```javascript
function sum(x, y) {
  if (y > 0) {
    return sum(x + 1, y - 1);
  } else {
    return x;
  }
}

sum(1, 100000)
// Uncaught RangeError: Maximum call stack size exceeded(…)
```

蹦床函数（trampoline）可以将递归执行转为循环执行。

```javascript
function trampoline(f) {
  while (f && f instanceof Function) {
    f = f();
  }
  return f;
}
```

## 10.属性的简洁表示法

```javascript
var foo = 'bar';
var baz = {foo};
baz // {foo: "bar"}

// 等同于
var baz = {foo: foo};
```

