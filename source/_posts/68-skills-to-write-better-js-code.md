---
title: 读书笔记：编写高质量javascript的68个方法
date: 2018-02-07 10:17:16
tags:
---

书还没看完。一遍看，一遍写读书笔记。

这本书的序是JavaScript之父Brendan Eich写的，作者是JavaScript标准化委员会专家。可想而知其质量如何。这本书不厚，和《JavaScript语言精粹》差不多厚，约等于4分之一的《JavaScript权威指南》的厚度。绝对值得一看。

# 1. 本书赞誉
本书的赞誉有来自Chrome开发主管，有来自JSHint的专家，还有一些行业大咖。

> 如果你想成为一名真正的JavaScript开发者, 那么请阅读这本书。就我来说，我多么希望在第一次开始JavaScript编程时就阅读它。---Anton Kovalyov, JSHint开发者

> 很少有人有机会同大师一起学习他们的手艺。这本书弥补了这种缺陷，其对JavaScript的研究就像随一位时间旅行哲学家回到公园前5世纪与柏拉图一起学习。---Rick Waldron, JavaScript传教士， Bocoup

# 2. 让自己习惯JavaScript
> 有些人说不清哪里好，可就是谁也替代不了。
## 2.1. 了解你使用的JavaScript的版本

## 2.2. 理解JavaScript的浮点数

## 2.3. 当心隐式的强制类型转换

## 2.4. 原始类型优于封装对象

## 2.5. 避免对混合类型使用 == 运算符

## 2.6. 了解分号插入的局限

## 2.7. 视字符串为16位的代码单元序列

# 3. 变量与作用域
> 作用域对程序员来说就像氧气。它无处不在，甚至，你往往不会去想它。但当它被污染时，你会感觉到窒息。

## 3.1. 尽量少使用全局对象
- 避免声明全局变量
- 尽量声明局部变量
- 避免对全局变量增加属性

## 3.2. 始终声明局部变量

## 3.3. 避免使用with语句

## 3.4. 熟练使用闭包
> JavaScript的函数值包含了比调用他们时执行所需要的代码还要更多的信息。而且，JavaScript函数值还在内部存储他们可能会引用的定义在其封闭作用域的变量。那些在其所涵盖的作用域内跟踪变量的函数称为闭包。

- JavaScript允许你引用在当前函数以外定义的变量
- 即使外部函数已经返回，当前函数仍然可以引用外部函数定义的变量
- 闭包可以更新外部函数的值

## 3.5. 理解变量声明提升
## 3.6. 使用立即调用表达式创建局部作用域
## 3.7. 当心命名函数表达式笨拙的作用域
## 3.8. 当心局部块函数声明笨拙的作用域
## 3.9. 避免使用evel创建局部变量
## 3.10. 间接调用eval函数函数优于直接调用