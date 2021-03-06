# 学习笔记 0531

## 关键字

```bash
len 长度
len(os.Args)

range 产生一堆值；索引以及在该索引处的元素值。

// 创建函数 make 和 new
make(T, args) 返回一个复杂的结构
counts := make(map[string]int)

new(T) 返回一个 `*T` , 返回一个指向已清零内存的指针
```

Go 语言中不允许使用无用的局部变量 (local variables), 会导致编译错误。
解决方法使用 `空标识符` 即 `_`

## 格式字符串

```bash
%d            十进制整数
%x, %o, %b    十六进制，八进制，二进制
%f, %g, %e    浮点数： 3.141593 3.141592653589793 3.141593e+00
%t            布尔：true或false
%c            字符（rune） (Unicode码点)
%s            字符串
%q            带双引号的字符串"abc"或带单引号的字符'c'
%v            变量的自然形式（natural format）
%T            变量的类型
%%            字面上的百分号标志（无操作数）
\t            制表符
\n            换行符
```

## 语法

import 了一个包路径包含有多个单词的 package 时，比如 image/color（image 和 color 两个单词）
通常用后一个单词表示这个包,例如 color.White
