# 痞子衡嵌入式半月刊： 第 73 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 72 期》](https://www.cnblogs.com/henjay724/p/17155192.html)

## 唠两句

历史上的今天：1782年3月12日，中国古代最大的文化工程《四库全书》编成。

本期共收录 4 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、Slint - 全开源跨平台UI设计库</font>

Slint 是一个工具包，可以有效地为任何显示器(嵌入式设备和桌面应用程序)开发流畅的图形用户界面。Slint支持多种编程语言，如Rust、c++和JavaScript。Slint 官方已经为 STM32 和 RP2040 做了适配。

> * 项目主页：https://github.com/slint-ui/slint

![](http://henjay724.com/image/biweekly20230312/Slint.PNG)

### <font color="red">2、MRI - 用于Cortex-M设备的gdb兼容调试监视器</font>

MRI 是一个调试监视器，它允许 GNU调试器 GDB 调试 Cortex-M3/M4 处理器。这使得使用功能齐全的源级调试器调试在 Cortex-M 设备上运行的应用程序成为可能，而不需要额外的硬件，只需一个串行连接。

> * 项目主页：https://github.com/adamgreen/mri

### <font color="red">3、Reflow-Controller - 全开源回流控制器</font>

Reflow-Controller 是一个回流控制器，用来控制不同种类的回流炉，热板等。它基于 ESP32-S2，因此可以编程为与 WiFi App 或其他应用程序一起使用。不过，它也有一个板载 OLED 显示屏和三个按钮，可以作为独立的解决方案使用。

> * 项目主页：https://github.com/makermoekoe/Reflow-Controller

![](http://henjay724.com/image/biweekly20230312/Reflow-Controller.PNG)

### <font color="red">4、ZSWatch - 基于 Zephyr 的开源智能手表</font>

ZSWatch 是一个基于Zephyr™ RTOS 的从零开始的全开源智能手表项目，包括硬件和软件。ZSWatch 项目分为两代：V1、V2，其中 V1 已经全部完成，V2 正在进行中。

> * 项目主页：https://github.com/jakkra/ZSWatch

![](http://henjay724.com/image/biweekly20230312/ZSWatch-1.PNG)

![](http://henjay724.com/image/biweekly20230312/ZSWatch.PNG)

## 工具类

### <font color="red">1、aardio - 专注于桌面软件开发的动态编程语言</font>

aardio 专注于桌面软件开发，17年一直保持非常活跃地更新，aardio 被多年用于生产项目实践，久经测试和锤炼。

> * 工具主页：https://www.aardio.com/

aardio 小、轻、快，轻便利索，体积仅 6.5MB，学习和使用成本极低。aardio 虽然小，但提供了惊人数量的开源标准库、扩展库 - 这些库基本都是由纯 aardio 代码实现，涉及到了桌面编程的方方面面。aardio 中的所有库基本都是由作者一个人编写，所以拥有良好的一致性。

区别于其他动态语言，aardio 可以非常方便地支持真多线程，并且提供大量多线程函数库、演示范例等等。

![](http://henjay724.com/image/biweekly20230312/aardio.png)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

