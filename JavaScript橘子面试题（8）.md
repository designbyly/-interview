## 1.`normalize`方法参数的四个可选值（不重要，了解）

- `NFC`，默认参数，表示“标准等价合成”（Normalization Form Canonical Composition），返回多个简单字符的合成字符。所谓“标准等价”指的是视觉和语义上的等价。
- `NFD`，表示“标准等价分解”（Normalization Form Canonical Decomposition），即在标准等价的前提下，返回合成字符分解的多个简单字符。
- `NFKC`，表示“兼容等价合成”（Normalization Form Compatibility Composition），返回合成字符。所谓“兼容等价”指的是语义上存在等价，但视觉上不等价，比如“囍”和“喜喜”。（这只是用来举例，`normalize`方法不能识别中文。）
- `NFKD`，表示“兼容等价分解”（Normalization Form Compatibility Decomposition），即在兼容等价的前提下，返回合成字符分解的多个简单字符。

## 2.includes(), startsWith(), endsWith()三者区别

- **includes()**：返回布尔值，表示是否找到了参数字符串。
- **startsWith()**：返回布尔值，表示参数字符串是否在源字符串的头部。
- **endsWith()**：返回布尔值，表示参数字符串是否在源字符串的尾部。

## 3.`indexOf`方法的作用什么

可以用来确定一个字符串是否包含在另一个字符串中。

## 4.说一下repeat()

`repeat`方法返回一个新字符串，表示将原字符串重复`n`次。

## 5.padStart()，padEnd()

ES7：字符串补全长度。如果某个字符串不够指定长度，会在头部或尾部补全。`padStart`用于头部补全，`padEnd`用于尾部补全。

## 6.听说过模板字符串吗

模板字符串（template string）是增强版的字符串，用反引号（`）标识。它可以当作普通字符串使用，也可以用来定义多行字符串，或者在字符串中嵌入变量。

## 7.String.raw()用来干什么

充当模板字符串的处理函数，返回一个斜杠都被转义（即斜杠前面再加一个斜杠）的字符串，对应于替换变量后的模板字符串。

## 8.在ES5中，RegExp构造函数的参数说明

第一种情况是，参数是字符串，这时第二个参数表示正则表达式的修饰符（flag）。

第二种情况是，参数是一个正则表示式，这时会返回一个原有正则表达式的拷贝。

## 9.字符串的正则方法有哪些

- `String.prototype.match` 调用 `RegExp.prototype[Symbol.match]`
- `String.prototype.replace` 调用 `RegExp.prototype[Symbol.replace]`
- `String.prototype.search` 调用 `RegExp.prototype[Symbol.search]`
- `String.prototype.split` 调用 `RegExp.prototype[Symbol.split]`

## 10,s 修饰符：dotAll 模式怎么理解

正则表达式中，点（`.`）是一个特殊字符，代表任意的单个字符，但是行终止符（line terminator character）除外。

以下四个字符属于”行终止符“。

- U+000A 换行符（`\n`）
- U+000D 回车符（`\r`）
- U+2028 行分隔符（line separator）
- U+2029 段分隔符（paragraph separator）

