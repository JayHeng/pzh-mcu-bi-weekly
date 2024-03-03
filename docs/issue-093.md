# 痞子衡嵌入式半月刊： 第 93 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 92 期》](https://www.cnblogs.com/henjay724/p/18024109)

## 唠两句

历史上的今天：

本期共收录 4 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、raspberry-pi-os - 学习使用Linux内核和树莓派开发操作系统</font>

此项目包含一个循序渐进的指南，教您如何从头开始创建一个简单的操作系统(OS)内核。作者称这个操作系统为树莓派操作系统或RPi操作系统。RPi操作系统的源代码主要基于Linux内核，但是该操作系统的功能非常有限，并且只支持Raspberry PI 3。

 * 项目地址：https://github.com/s-matyukevich/raspberry-pi-os

### <font color="red">2、MiniLisp - 1K行C语言写的Lisp解释器</font>

有一天，项目作者想看看用1000行C代码能做些什么，于是决定写一个Lisp解释器，这变成了一个有趣的周末项目，结果是一个迷你lisp实现。所有这些都在1000行c中，作者没有为了大小而牺牲可读性。在作者看来，代码中有大量注释，以帮助读者理解所有这些特性是如何工作的。

 * 项目地址：https://github.com/rui314/minilisp

MiniLisp 实现了整数、符号、局部变量、条件语句、宏和垃圾回收等功能。

### <font color="red">3、Zstandard - 快速无损的数据压缩算法Zstandard的实现</font>

Zstandard，简称 zstd，是一种快速无损压缩算法，针对 zlib 级的实时压缩场景和更好的压缩比。在相似的压缩比情况下，它解压缩的速度比其他的算法都要快。很多知名项目都有这个算法的身影。

 * 项目地址：https://github.com/facebook/zstd

如下表是使用 lzbench (@inikep使用gcc 9.3.0编译的开源内存基准)在 Silesia 压缩语料上测试和比较了几种快速压缩算法：

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-093/Zstandard.PNG)

### <font color="red">4、linq4c - C#的linq方法之C实现</font>

C# LINQ（Language Integrated Query）是一种强大且灵活的查询语言，可以将数据查询、过滤、排序和转换等操作无缝集成到 C# 代码中。如果你想在 C 中使用 C# 的 linq 方法，那么不妨来使用这个项目！这是它的 C 语言版。实现了 linq 的大部分方法（60+）。

 * 项目地址：https://github.com/haifenghuang/linq4c

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

