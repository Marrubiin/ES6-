ES6学习笔记

1.变量let和const，使用let替代var，理解作用域。使用const申明常量。

2.do表达式，获取块级作用域的返回值

3.解构赋值：数组、对象、字符串、数值和布尔值、函数参数

用途：(1)交换变量的值 (2)函数返回多个值 (3)定义函数的参数 (4)提取JSON数据 (5)设置函数默认值 (6)遍历Map结构 (7)加载模块时指定方法
  
4.Unicode字符扩展，识别超出\u0000~\uFFFF之间的字符

(1)codePointAt()，返回指定位置的字符编码，codePointAt(0)返回特殊字符的完整编码，从1开始和charCodeAt()返回相同。es5的方法为charCodeAt()。

(2)String.fromCodePoint()，从码点返回对应字符，可识别32位的UTF-16字符(Unicode编号大于0xFFFF)，es5方法Strign.fromCharCode的扩展。

(3)字符串遍历方法for...of

(4)at()，返回字符串指定位置的字符，es5方法为charAt()。

(5)normalize()，统一字符的不同表示方法，Unicode正规化。

5.字符串查找方法：includes()、startWith()、endsWith()。

includes()：判断是否找到字符串，startWith()：判断字符串是否在原字符串头部，endsWith()：判断字符串是否在原字符串尾部。

三个方法都可使用第二个参数，表示开始搜索的位置。

6.repeated()，第一个参数为需要重复的字符串，第二个字符串为重复的次数。大-1的小数会自动取整，小于1的书或者Infinity会报错。NaN等于0。字符串会自动转换为数字。

7.padStart()，padEnd()：用指定字符串补齐到指定长度，第一个参数为长度，第二个为补齐字符串。省略第二个参数，会使用空格补齐。可指定字符串格式。

8.模板字符串，使用反引号表示，变量使用$()格式。取消换行或者空格格式，可以使用trim()方法

9.RegExp构造函数

ES6允许使用第二个参数作为正则表达式修饰符，返回结果会忽略原先的修饰符。

字符串的正则表达式：match()、replace()、search()、split()

10.数值的扩展

(1)二进制和八进制表示法： ES6提供了二进制和八进制新写法，二进制前缀0b/0B，八进制前缀0o/0O。转换为十进制使用Number()方法。

(2)Number.isFinite()：检查一个数值是否为有限的；
Number.isNaN()：检查一个值是否为NaN；
Number.parseInt()：转换为整型；
Number.parseFloat()：转换为float类型；
Number.isInteger()：判断一个值是否为整数；
Number.EPSILON：常量，表示1与大于1的最小浮点数之间的差，用于处理浮点数之间的运算；
Number.MAX_SAFE_INTEGER和Number.MIN_SAFE_INTEGER：整数上下限（-2^53到2^53）；
Number.isSafeInteger()：判断一个整数是否在上面变量的范围内。

(3) Math对象
Math.trunc():去除小数的小数部分，返回整数部分；
Math.sign()：判断一个数是正数(+1)、负数(-1)还是零(0)，其他返回NaN；
Math.cbrt()：计算一个数的立方根；
Math.clz32()：返回一个数的32位无符号整数形式有多少个前导0；
Math.imul()：返回两个数以32位带符号整数形式相乘的结果；
Math.fround()：返回一个数的单精度浮点数形式；
Math.hypot()：返回所有参数的平方和的平方根；
对数；双曲函数；
Math.signbit()：判断一个数是否有符号位，NaN返回false，-0返回true，负值返回true，其他返回false；

(4)指数运算符(**)

(5)Integer数据类型：取消精度对整数的影响，使用后缀n，运算方法和普通运算方法一致，/运算会舍去小数部分。

11.函数的扩展

(1)可给函数的参数指定默认值

(2)有默认值的参数应放在函数尾部

(3)函数的length属性，返回没指定默认值的参数个数

(4)rest参数，格式(...values)，获取函数的多余参数，可替代arguments对象

(5)ES6规定，函数参数使用了默认值、解构赋值或扩展运算符，则不能在函数内部设定严格模式

(6)name属性，返回函数名

(7)箭头函数(=>)


