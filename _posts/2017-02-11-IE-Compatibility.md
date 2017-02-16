---
layout: post
title: "关于这次项目做的IE兼容性的解决方案"
description: "在vue和一些不兼容IE8的js框架下的一种项目解决方案"
date: 2017-02-11 18:39:18
comments: true
keywords: "关于IE兼容方案"
category: dev
tags:
- IE compatibility
---

在最近做的前端项目中，做了一个浏览器兼容方案，但是在IE8，9下提示出不来。

原来原因是一些不兼容低版本浏览器和js依赖模块的语法报错，由于引入不兼容的脚本框架过多，导致js报错，连提示页面的进不去。领导提出的方案是将提示页改成兼容IE低版本的浏览器。做的过程中发现这个方案不可行。

于是，找到了另外一种解决方案。<a target="_blank" href="http://www.cnblogs.com/fm168/p/5526702.html">用条件判断IE版本</a>