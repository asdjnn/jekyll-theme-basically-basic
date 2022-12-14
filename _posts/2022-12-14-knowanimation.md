---
title: "CSS过渡变形和动画"
layout: page
read_time: true
image: assets/image/banner/note.jpg
categories: 
  - 学习笔记
author: 
  name: 陈星灿
---

### 过渡
* 为元素从一种样式转变为另一种样式时添加效果，例如渐显、渐弱、动画快慢等。

#### transition-property属性：
* transition-property 属性用于指定应用过渡效果的CSS属性的名称。
基本语法格式：transition-property: none | all | property;

#### transition-duration属性
* transition-duration属性用于定义过渡效果花费的时间，默认值为0，常用单位是秒（s）或者毫秒（ms）
基本语法格式：transition-duration:time;

#### transition-timing-function属性
* transition-timing-function属性规定过渡效果的速度曲线，默认值为“ease“
基本语法格式：transition-timing-function:linear|ease|ease-in|ease-out|ease-in-out|cubic-bezier(n,n,n,n);

#### transition-delay属性
* transition-delay属性规定过渡效果何时开始，默认值为0，常用单位是秒（s）或者毫秒（ms）
基本语法格式：transition-delay:time;
正数:过渡动作会延迟触发。
负数：过渡动作会从该时间点开始，之前的动作被截断。

#### transition属性
* transition属性是一个复合属性，用于在一个属性中设置transition-property、transition-duration、transition-timing-function、transition-delay四个过渡属性。
基本语法格式：transition：property duration timing-function delay;

### 变形
* css3变形包括：平移，旋转，缩放，倾斜
基本语法格式：transform：none （不变形）| transform-functions（变形函数或变形函数列表）transform-functions函数

#### 中心点
* 变形操作都是以元素的中心点为基准进行的，如果需要改变这个中心点，可以使用transform-origin属性。
基本语法格式：transform-origin: x-axis y-axis z-axis;
属性参数：
transform-origin属性包含三个参数，其默认值分别为50% 50% 0，各参数的具体含义

#### 平移
* transform:translate（x-value,y-value）;
说明：x-value指元素在水平方向上移动的距离，y-value指元素在垂直方向上移动的距离。如果省略了第二个参数，则取默认值0。当值为负数时，表示反方向移动元素

#### 缩放
* transform:scale(x-axis,y-axis);
说明：x-axis和y-axis参数值可以是正数、负数和小数。正数值表示基于指定的宽度和高度放大元素。负数值不会缩小元素，而是反转元素（如文字被反转），然后再缩放元素。如果第二个参数省略，则第二个参数等于第一个参数值。

### 动画
* animationname：表示当前动画的名称，它将作为引用时的唯一标识，因此不能为空。
keyframes-selector：关键帧选择器，即指定当前关键帧要应用到整个动画过程中的位置，值可以是一个百分比、from或者to。其中，from和0%效果相同表示动画的开始，to和100%效果相同表示动画的结束。
css-styles：定义执行到当前关键帧时对应的动画状态，由CSS样式属性进行定义，多个属性之间用分号分隔，不能为空。