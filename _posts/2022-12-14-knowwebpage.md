---
title: "响应式网页与媒体查询"
layout: page
read_time: true
image: assets/image/banner/note.jpg
categories: 
  - 学习笔记
author: 
  name: 陈星灿
---

### 什么是媒体查询
* RWD利用弹性网格布局(fluid grid)、弹性图片／媒体(flexible images)、媒体查询(media queries)等技术实现。
利用媒体查询，可以根据设备的能力应用特定的CSS样式。比如，根据视口宽度、屏幕宽高比和朝向（水平或垂直），只用几行CSS代码就改变内容的显示方式。
媒体查询包含媒体类型和零个或多个检测媒体特性的表达式。Width、height和color都是可用于媒体查询的特性。使用媒体查询，可以不必修改内容本身，而让网页适配不同的设备。

### 断点
* 断点就是某个宽度临界点。跨过这个点布局就会发生显著变化。断点应该由内容和设计本身决定，而不是有固定的设备断点。

### 媒体查询可以测试哪些特性？
* 媒体查询用的最多的特性是视口宽度（width），很少需要用到其他特性（偶尔会用到分辨率和视口高度）。
Width：视口宽度
Height: 视口高度
Device-width：渲染表面的宽度（设备屏幕宽度）
Device-height:渲染表面的高度（设备屏幕宽高度）
Orientation：设备方向是水平还是垂直
Aspect-ratio：视口的宽高比。aspect-ratio：16/9
Color：颜色组分的位深。
Color-index: 设备颜色查找表中的条目数。
Resolution: 屏幕或打印分辨率。
Scan：针对电视的逐行扫描和各行扫描。
Grid：设备基于栅格还是位图。 