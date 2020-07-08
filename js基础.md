# js基础

---
####1、数据类型
> js存在8种数据类型（7种原始类型和1种引用类型）
> 数据类型：number、bigint、boolean、string、null、undefined、symbol
> 引用类型：object

####2、类型转换
> （1）字符串转换：可显式调用 `String(value)` 来将value转换为字符串类型
> ```
> typeof(String(false)) // string
> typeof(String(true))  // string
> typeof(String(null))  // string
> ```
>
> （2）数字型转换：算数函数和表达式中，会自动进行number类型转换；也可使用`Number(value)`进行number类型转换
> ```
> 转换规则：
> undefined --> NaN
> null --> 0
> true/false --> 1/0
> string --> 去掉首尾空格后的纯数字字符串中含有的数字。如剩余字符串为空，则转换结果为0。否则将会从剩余字符串中读取数字。当类型转换出现error时返回NaN。如下：
> Number("  1213  ")  --> 123
> Number("123z") --> NaN (读取到‘z’时出现error)
> ```
>
> 布尔型转换：发生在逻辑运算中，可通过Boolean(value)显式地进行转换
> ```
> 转换规则：
> 0、null、undefined、NaN、""  --> false
> 其他值 --> true
> ```





