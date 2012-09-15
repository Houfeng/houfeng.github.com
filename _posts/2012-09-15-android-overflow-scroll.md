---
layout: post
title: 移动web开发局部区域滚动问题
published: true
---
###问题
开发一个针对pc的web应用时，在需要不随内容滚动的页头或面页脚时，通常的做法是如下样式：

> .ui-head{ position:fixed; }

但是如上的样式放到手机上，我测试过android2.x、android4.x、ios4.x皆不支持position:fixed;

但经过测试，发现ios5.x已经支持position:fiexd,但通过position:fiexd一般只能实现页整的整体滚动时页头或页脚的固定，在实现页面某一小区域的滚动效果还是不太方便。

###通过webkit特有的样式实现
经测试ios5.1已支持如下样式定义：

> -webkit-overflow-scrolling: touch;

通过如上定义，ios5.x可以样式（不用js）实现局部区域滚动；但目前我试过android2.x及android4.x发现依然不支持些样式。

###通过javascript实现
为了实现兼容主流平台及浏览器，常见的做法（很多web开发框架就是依赖javascript实现）

未写完……























