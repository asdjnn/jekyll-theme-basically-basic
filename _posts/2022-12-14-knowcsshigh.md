---
title: "CSS高级技术"
layout: page
read_time: true
categories: 
  - 学习笔记
author: 
  name: 陈星灿
---

### 使用CSS3制作文字阴影
* text-shadow属性：在CSS3中可以用text-shadow属性给页面上的文字添加阴影效果,可以通过对text-shadow属性设置相关的属性值，来实现一些需要的字体阴影效果,减少了图片的使用。
text-shadow属性的使用方法：text-shadow：X轴Y轴Rpxcolor;
属性说明（顺序依次对应）：阴影的X轴(可以使用负值)阴影的Y轴(可以使用负值)阴影模糊值（半径大小）阴影的颜色。

* 位移距离：text-shadow所使用的参数中，前两个参数是阴影离开文字的横方向和纵方向的位移距离，使用的时候必须指定这两个参数；
* 阴影的模糊半径：text-shadow属性的第三个参数就是阴影模糊半径，代表阴影向外模糊时的模糊范围；
* 阴影的颜色：text-shadow属性的第四个参数就是绘制阴影时所使用的颜色，可以放在三个参数之前，也可以放在三个参数之后。当没有指定颜色值的时候，会使用文本的color颜色值。

### 使用CSS3制作盒阴影
#### box-shadow的语法结构：
* box-shadow: h-shadow v-shadow blur spread color inset;
h-shadow：水平阴影的偏移值，必需，可以为负值。
v-shadow：纵向阴影的偏移值，必需，可以为负值。
blur：阴影模糊值，可选，不能为负值。
spread：阴影的扩展，可选，可以为负值。
color：阴影的颜色，虽然是可选，但是在不同的浏览器里面解释不一样，有些是黑色，有些是透明，所以建议都要设置。具有透明度的阴影可以用rgba的值。
inset：内阴影。可选，如果缺省，默认是外阴影（outset）