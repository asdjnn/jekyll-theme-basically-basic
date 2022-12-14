---
title: "CSS新特性"
layout: page
categories: 
  - 学习笔记
author: 
  name: 陈星灿
---

# CSS新特性
### 多列布局（Multi-column）
* 多列布局就是将文本内容设计成像报纸那样的多列布局。或者说在之前我们通过js或者JQuery才能实现的瀑布流，在CSS3中我们可以直接通过CSS就可以实现，虽然有兼容性上面的问题。

* 多列布局的属性
columns：设置对象的列数和每列的宽度。是复合属性。
column-width：设置对象没列的宽度。
column-count：设置列数
column-gap：设置列与列之间的间隙
column-rule：设置列与列之间的边框（我更喜欢称为分割线），复合属性。
column-span：设置元素是否跨所有列。
column-fill：设置对象所有列的高度统一（目前主流浏览器都不兼容）。（排版）
column-break：设置换行，复合属性，有3个子属性。

### 断字
* 截断文字
比如有下面标记，

 `<p class`="truncate">OK, listen up, I've figured out the key eternal happiness. All you need to do is eat lots of scones.`</p >`

但我们想让它在520px像素宽的容器里显示成这样：
OK, listen up, I've figured out the key eternal happiness. All you n...

* 以下是实现这一效果的CSS：
```
.truncate {
 width: 520px;
 background-color: #03A66A;
 overflow: hidden;
 text-overflow: ellipsis;
 white-space: nowrap;
}

```
* 只要内容超过既定宽度（如果是在一个弹性容器里，可以设置为10%），就会被截短。
text-overflow: ellipsis;   表示显示省略符号来代表被修剪的文本。
最后的white-space:nowrap声明是为了确保长出来的文本不会折行显示在外部元素中。