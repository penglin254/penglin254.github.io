---
layout: post
title: "关于vue的checkbox的ie兼容性问题"
description: "关于vue的checkbox的ie兼容性问题，以及解决方法"
date: 2017-01-20 20:39:18
comments: true
keywords: "vue,关于vue的checkbox的ie兼容性问题，以及解决方法"
category: dev
tags:
- vue checkbox
---

在最近的开发过程中，调试IE的兼容性问题。发现了vue2的版本中,checkbox的一个bug,在IE11下，点击多次，有时候绑定失效的问题。同时@click和v-model不能同时使用。

经过多次调试，在IE11下的解决方案如下

用:value取代v-model