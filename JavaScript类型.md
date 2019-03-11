# JavaScript类型

## 类型

JavaScript 语言规定了 7 种语言类型。

*  Undefined（未定义）
*  Null（空）
*  Boolean（布尔）
*  String（字符串）
*  Number（数字）
*  Symbol（符号）
*  Object（对象）
    * Function（函数）
    * Array（数组）
    * Date（日期）
    * RegExp（正则表达式）

## Undefined、Null

undefined是一个变量，null是一个关键字（true 和 false 两者都是关键字）

```
为什么有的编程规范要求用 void 0 代替 undefined？
void的返回值都是undefined。
在ES5之前，window下的undefined是可以被重写的。
在ES5之后，规定了全局变量下的undefined值是不能被配置（non-configurable），不能被重写（non-writable）的，但是局部变量中依然可以对之进行改写。
这是 JavaScript 语言公认的设计失误之一，所以，我们为了避免无意中被篡改，建议使用 void 0 来获取 undefined 值。
```