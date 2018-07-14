---
layout: post
title:  "回调函数的事件轮询机制"
categories: SnakeSon
tags:  event
author: LiuChaofanw
---
```	js
    heap：堆
   	stack：栈
   	event loop：事件轮询
   	callback queue：回调队列
   	事件轮询：由于js是代码是单线程执行的，但是有分线程的支持。浏览器的管理模块就运行在分线程，其中包括3部分：DOM事件管理模块、ajax请求管理模块、定时器管理模块。当异步回调函数被触发之后，浏览器的管理模块就会将该回调函数添加到回调队列中。当主线程执行完同步的js代码之后，就会开始执行回调队列中的回调函数。

/usr/share/applications
```
![](https://i.imgur.com/I6KTOeE.png)

