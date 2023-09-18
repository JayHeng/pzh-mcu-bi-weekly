# 痞子衡嵌入式半月刊： 第 80 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 79 期》](https://www.cnblogs.com/henjay724/p/17591452.html)

## 唠两句

历史上的今天：1931年，九一八事变爆发。

本期共收录 3 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、mr-library - 一个专为嵌入式系统设计的轻量级框架</font>

mr-library 是一个专为嵌入式系统设计的轻量级框架，模块化的软件架构充分考虑了嵌入式系统的资源和性能要求。 通过提供标准化的设备管理等，极大地简化了嵌入式应用的开发难度，帮助开发者快速构建嵌入式应用程序。

**设备框架** 为开发者提供标准化的接口（open、close、ioctl、read、write），解耦应用程序与底层硬件驱动，使应用开发无需硬件驱动的实现细节。 当硬件变动时，只需要适配底层驱动，上层应用可以无缝地迁移到新硬件上，大大提高了软硬件的可重用性和可扩展性。

> * 项目地址：https://gitee.com/MacRsh/mr-library

mr-library 应用场景:

```text
- MCU开发中硬件（gpio、uart、spi、i2c、pwm等）标准化管理。
- RTOS实时操作系统的外挂设备框架。
- 各类Iot和智能硬件产品的快速开发。
```

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-080/mr-library.png)

### <font color="red">2、c-periphery - 在Linux中用于外围设备访问C库</font>

c-periphery是一个小型 C 库，用于在用户空间 Linux 中进行 GPIO，LED，PWM，SPI，I2C，MMIO 和串行外围设备 I/O 接口访问。 c-periphery 简化了本机 Linux API 并将其整合到这些接口。  

c-periphery 在嵌入式 Linux 环境（包括 Raspberry Pi，BeagleBone 等平台）中可用于与外部外围设备接口。 c-periphery 是可重入的，在标准C库和Linux之外没有任何依赖关系，可编译成静态库以方便与其他项目集成。  

> * 项目地址：https://github.com/vsergeev/c-periphery

### <font color="red">3、linkboy - 自研的编程语言和集成开发环境</font>

LinkBoy 是自研的编程语言和集成开发环境，主要面向中小学信息技术教育，也用于大学工科教学，以及帮助工控、电子工程师快速开发构建项目。LinkBoy 作者王强老师于 2009 年在大学时率先启动该项目，因当时大学里普遍在用国外的 keil 等收费编程软件进行教学，于是王强立志开发一款国产的编程语言和环境。后来随着应用场景的不断深入，逐步增加图形化界面、IoT 库、软件仿真器等功能。

> * 软件官网：http://linkboy.cc/
> * 项目地址：https://gitee.com/linkboy_crux/linkboy

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-080/linkboy.PNG)

LinkBoy 是生成自研编程语言程序代码，从源程序词法语法分析到后端机器码烧录文件的生成均是自主开发，并与图形界面做整合，因此可以支持图形界面的连线配置，程序的拟物化模拟仿真运行。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-080/linkboy2.PNG)

## 工具类

### <font color="red">1、SourceTrail - 可视化源代码编辑神器</font>

 Sourcetrail 是一个免费开源、跨平台的可视化源码编辑器。不同于其他代码编辑器的导航栏， Sourcetrail 左侧使用图形直观地表示了调用上游和下游，类成员列表等等细节，使得理解源代码的结构变得很容易。目前支持 C、C++、Python 和 Java 语言，同时提供了相关 SDK 用于拓展支持其它语言。

> * 软件官网：https://www.sourcetrail.com/

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-080/sourcetrail.png)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

