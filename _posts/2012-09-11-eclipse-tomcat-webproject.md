---
layout: post
title: eclipse+tomcat web工程引用其它工程
category: 闲谈
published: true
---

> 之前用eclipse做android开发的时候，一个工程项目引用的方式引用另一个工程，一直没有问题。今天为一个web工程引用另一个工程的时候，编译运行发生找不到“类”的错误。

###解决方法
1.选中web工程
2.按下alt键
3.按下enter键

会弹出如下对话框:
![](http://img8.ph.126.net/ODPFlUgMkr_OKj_FAEvahg==/108367866051026258.jpg)

最后:
在Deployment Assembly中添加要引用的项目即可。