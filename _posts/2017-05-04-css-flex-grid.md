---
layout: post
title: "css grid布局"
description: "grid布局，flex对比，为什么要用网格布局"
date: 2017-05-04 18:39:18
comments: true
keywords: "css grid布局"
category: dev
tags:
- css grid
---

1.为什么要用网格布局

在一个web网页中，可以分割成多个内容块，而这些内容块都占据自己的区域(regions)，可以将这些区域看成是一个虚拟的网格。到目前为止，在一个模板中使用不同的结构标签，使用多个浮动和手动计算实现一个布局。这对于Web前端人员来说，这是一件痛苦之事。而网格布局将让你摆脱这样的困局，让你的布局方法变得非常简单与清晰。

2.浏览器兼容性

<img src="../img/css-grid.png">

仅在IE10+上支持，而且也仅支持部分属性。

3.使用

(1).网格线

网格线组成了网格，他是网格的水平和垂直的分界线。

(2).网格轨道

好比表格中的行或列，网格中其分为grid column和grid row。每个网格轨道可以设置一个大小，用来控制宽度或高度。

(3).网格单元格

网格单元格是指四条网格线之间的空间。所以它是最小的单位，就像表格中的单元格。（table cell）

(4).网格区域
网格区域是由任意四条网格线组成的空间，所以他可能包含一个或多个单元格。相当于表格中的合并单元格之后的区域。

4.注意事项

    display:grid or display:inline-grid; //使用网格布局
    多列布局模块中的所有column-*属性运用在网格容器上将失效
    float和clear使用在网格项目（网格单元格Grid Cell）上将失效
    vertical-align使用在网格单元格上将失效
    ::first-line和::first-letter这样的伪元素不能应用在网格容器上
    
5.设置

(1).chrome

#enable-experimental-web-platform-features），一个更为简单的方法，可以直接在浏览器地址栏中输入网址：chrome://flags#enable-experimental-web-platform-features立马定位需要的选项，然后点击“启用”(enable)按钮，

(2).同上