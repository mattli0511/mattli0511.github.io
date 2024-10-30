---
layout: post
title:  "我电脑上的FydeOS"
date:   2024-10-20 00:18:00 +0800
categories: article
---

众所周知，FydeOS是Chromium中较为成功本地化的一个系统，并且它比较轻量化UI也比较简洁。因此，我就想把它装到我自己的电脑上，体验一把FydeOS的魅力。

# 写在前面

需要注意的是，我这台笔记本的一些配置与你的可能有不同，因此最终的体验也难免会有不同。

本文中的FydeOS版本号为`FydeOS for PC(iris), 18.1`，版本不同体验亦可能不同。

# 主系统

FydeOS常被称为是本地化的Chrome OS[^1]，它最主要的部分自然是浏览器。不过，我们也可以先看看主系统的其余部分。

## 无关紧要的部分

![主界面](https://sway.cloud.microsoft/s/Zn4fzwS10dwauGAc/images/Yq15U8dDL5WlPC "主界面")

FydeOS的主界面的确简约，甚至可以说是简陋了。它没有什么铺满的图标，也没有什么可以把玩的小工具——它只是一个背景。

![日历](https://sway.cloud.microsoft/s/Zn4fzwS10dwauGAc/images/2rxtUM48PylcQi "日历")

一个纯正的日历，除了用来看星期几，大概是没有其他用处了。

![状态栏](https://sway.cloud.microsoft/s/Zn4fzwS10dwauGAc/images/LiU7OtnbyWJoCm "状态栏")

可以比较清晰地了解当前日期、时间、打开过的应用等等，实用价值还是有的。

![控制中心](https://sway.cloud.microsoft/s/Zn4fzwS10dwauGAc/images/e5hmVXZGHt4R88 "控制中心")

这个控制中心可以控制WiFi、蓝牙等参数，甚至可以控制关机，但由于未知原因，在我的这台电脑上，亮度实际上是不能调节的。

![通知中心](https://sway.cloud.microsoft/s/Zn4fzwS10dwauGAc/images/4feJaqCLt1WgyL "通知中心")

这通知中心，嗯，有一股安卓味儿了。

![通知窗口](https://sway.cloud.microsoft/s/Zn4fzwS10dwauGAc/images/4VsZFsUrpJUTbY "通知窗口")

值得注意的是，下载的时候，会单独弹出一个通知窗口。 ~~更像安卓了~~

![手写板](https://sway.cloud.microsoft/s/Zn4fzwS10dwauGAc/images/-oftT3xV_rZVYd "手写板")

没错，FydeOS也是有手写板的，不过我的电脑不支持触屏，只能鼠标写了。 ~~反正即使我真手写字也丑~~

## 主角——浏览器

刚点进来，我就有了一种熟悉的感觉：果然是Chromium生的，跟Chrome十分 ~~甚至九分~~ 的像。对于对Chrome比较熟悉的我来说，确实就没有太大的不适应感了。同时，这里也体现了FydeOS的本土化——主页默认是必应。

![开始页](https://sway.cloud.microsoft/s/Zn4fzwS10dwauGAc/images/RYKx1NaBu85Boa "开始页")

除去这部分，基本上就难以再找到什么区别了……**吗？**

其实还有几个小细节，等着你去发现。这些改变，大多是因FydeOS的性质以及本地化的需要而改变的，毕竟FydeOS终究不是Chrome OS。

![细节](https://sway.cloud.microsoft/s/Zn4fzwS10dwauGAc/images/OJLigtWp294kSO "不知道你有没有找到")

当然，设置里也有一些地方与Chrome不同，让你知道这可是另一个操作系统。

## （最重要的）配角——文件管理

众所周知，文件管理是一个系统相当重要的部分，毕竟存储文件本身就是使用电脑的一个目的。FydeOS的文件管理器延续了系统的设计语言，但又与安卓的有所不同。

![文件管理](https://sway.cloud.microsoft/s/Zn4fzwS10dwauGAc/images/d7hYejDSIi2s9o "文件管理")

在左侧，各个位置被一一列举出来，不同类别用一条横线分开。如果你在之前已经开启了OneDrive或者坚果云的服务，大概率它们也会出现在其中；在右侧，则罗列出了当前目录的所有文件。你可以改变文件的排列方式、顺序等，这点跟在安卓上差不多。

值得注意的是，用官方的文件管理器是**不能够**直接删除文件的，要先将文件移入回收站，然后再删除，这一点与安卓不同；如果移入回收站超过30天，系统就会帮你自动清除，Windows有这个功能，但是那是需要你认为开启的，大概你也没有开吧。

# Linux

啥，这啥也不是的系统，还能装Linux？

别说，FydeOS还真有一个Linux子系统（反正我这么叫），启动也比较轻松。当然，需要注意的是，它终究还是一个“虚拟机”。不过，里面的部分文件（再准确来说，目录）是共享的，所以两个系统间文件的交换不至于把人搞得焦头烂额。

FydeOS已经为你搞好了WPS和Vim[^2]，但是这只是一个稍微装修了一点的毛坯房，还有很大的“留白”，大家可以根据自己的需求，利用Linux的命令来安装更多的软件（记住要跟Debian走）。同时，那些有图形界面的软件依旧会在应用栏里的“Linux 应用”里显示，就像正常的应用一样。

我个人感觉，这里面的自带应用确实有些少了，甚至有些对于其他系统已经预装的软件都找不到，不过考虑到被分配的内存也不多，这么做也不是没有道理。看来，关键时刻还是得“自己动手，丰衣足食”啊。

# ~~Android~~

事实证明，这些安卓相关的软件在我的电脑上跑不起来，大概跟电脑配置有关系。

# 写在后面：我为什么用FydeOS

1. FydeOS相当轻量化，在我的这台电脑上，除了跑Android程序，几乎找不到卡的时候。
2. 有些时候，我想要稍微脱离那些专业的学习软件。
3. Chrome OS的风格我个人比较喜欢。

# 注释

[^1]:谷歌的一款系统，也是Chromium的一个分支。
[^2]:一个依托命令行运行的文字编辑软件。