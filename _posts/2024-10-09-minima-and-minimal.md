---
layout: post
title:  "GitHub Pages小笔记：Minima和Minimal傻傻分不清？"
date:   2024-10-09 19:36:45 +0800
author: Matt Li
categories: note
tag: GitHub Pages
---
熟悉GitHub Pages和jekyll的人都知道，GitHub Panges是可以更换主题的。不知道大家在捣鼓这个的时候，有没有犯过一个这样的错误——想换回默认主题的时候，在那一栏写的minimal，但最后却报了错。

没错，我就犯了这样的错误，犯了错仔细一看，才发现，原来不是**Minimal**，而是**Minima**。

那么，今天，我们就来看一下这两者有什么区别。

## 外观

在外观上，这两个主题就已经显现出了不同。

虽然都是走简约风，但是可以明显的发现，Minima将标题放在了页面顶端，而Minimal则将其放在了左端（当然，受限于屏幕尺寸，在手机端，二者的标题都在顶端）。

在一些细节上，两者也有些许不同，比如说，Minima的代码块的背景颜色偏蓝，而Minimal的代码块背景颜色是灰色。Minima的表格仍有行间白灰相间的背景颜色和明显的单元格边框，而Minimal仅在每行之间有分割线。

同时，Minima在顶端设置了一个列表，列举了一些页面，让人可以较为方便地去到一些没有列进博文列表的页面。Minima还可以设置主题 ~~（主题中的主题）~~。

## 位置

Minima和Minimal在GitHub中的位置的不同比较隐蔽，但我个人认为，这个区别更为重要。

Minima**直接属于jekyll**，也是安装jekyll后网页默认的主题。也就是说，你在建站的时候，基本上不需要特意地调用这个主题。当然，如果你要调节里面的一些参数，就需要另外再折腾了，具体怎么折腾，就去官方网站上查阅吧。

Minimal则**在pages-themes里面**，在调用的时候，需要特别地改一下`_config.yml`里面的设定。之后，根据官方教程，你还要调用命令行输入`gem "github-pages", group: :jekyll_plugins`，才可以用上这个主题。

## P. S.

这篇文章并未着重推荐某个主题，而且也不是只有两个主题可以选（像我就选了另一个主题）。在编辑网站的时候，最重要的还是个人偏好。

## 参考/相关链接

1. [Minima首页](https://github.com/jekyll/minima)
2. [Minimal首页](https://github.com/pages-themes/minimal?tab=readme-ov-file)