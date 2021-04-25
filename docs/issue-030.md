# 痞子衡嵌入式半月刊： 第 30 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 29 期》](https://www.cnblogs.com/henjay724/p/14645915.html)

## 唠两句

这周二是谷雨，历史上的今天：

本期共收录 0条资讯、1个项目，3个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、</font>



## 项目类

### <font color="red">1、libopencm3 - 开源Cortex-M系列单片机固件库</font>

libopencm3 项目（以前称为libopenstm32）旨在为各种ARM Cortex-M0（+）/M3/M4微控制器创建一个免费开源（LGPL v3或更高版本）的固件库。

> 项目主页: https://github.com/libopencm3/libopencm3

libopencm3 库当前支持的MCU包括但不限于:

```text
- ST STM32 F0xx/F1xx/F2xx/F30x/F37x/F4xx/F7xx/H7xx series
- ST STM32 G0xx G4xx L0xx L1xx L4xx series
- Atmel SAM3A/3N/3S/3U/3X series, as well as SAMDxx and friends
- NXP LPC1311/13/17/42/43
- Stellaris LM3S series (discontinued, without replacement)
- TI (Tiva) LM4F series (continuing as TM4F, pin and peripheral compatible)
- EFM32 Gecko series (only core support)
- Freescale Vybrid VF6xx
- Qorvo (formerly ActiveSemi) PAC55XX
- Synwit SWM050
```

该固件库完全是根据MCU厂商的数据表、编程手册和应用程序说明从头开始编写的。代码配合ARM GCC工具链一起使用，可以使用OpenOCD ARM JTAG软件将代码下载到MCU。

![](http://henjay724.com/image/biweekly20210425/.PNG)

## 工具类

### <font color="red">1、Serial Studio - 跨平台、多功能串行数据可视化程序</font>

Serial Studio是一个多平台，多用途的串行数据可视化的应用软件。Serial Studio的目标是使嵌入式开发人员和制造商可以轻松地可视化的呈现和分析其项目和设备生成的数据，而无需为每个项目编写专用的计算机软件。

> 软件主页: https://github.com/Serial-Studio/Serial-Studio

![](http://henjay724.com/image/biweekly20210425/Serial-Studio.gif)

Serial Studio采用JSON “映射”文件，创客们可以根据自身的需要来定制自己的控制面板接口，使用插件来显示他们的数据并导出所有接收到的信息到CSV/Excel格式，并有时间戳来标记每一帧的信息。Serial Studio可以扩展支持几乎所有与数据采集/测量相关的项目。

### <font color="red">2、SerialPlot - 简单易用的开源串口波形软件</font>

SerialPlot是一个可视化的串口收发工具，QT源码开源。这个软件非常好用，能录波、缩放、多种格式输入，数据输入设置比较灵活，作者还在持续更新。

> 软件主页: https://github.com/hyOzd/serialplot

![](http://henjay724.com/image/biweekly20210425/SerialPlot.gif)

### <font color="red">3、VOFA+ - 插件驱动的高自由度上位机</font>

VOFA+ 是一款通过直观简洁的协议将字节流翻译成多通道数据的软件，支持十六进制浮点数据，也支持CSV格式字符串流。VOFA+ 通过拖动的操作逻辑动态添加控件，并将数据绑定到控件上，以实现传感器数据的可视化。

> * 软件主页: https://www.vofa.plus/
> * 插件库： https://github.com/je00/Vodka

VOFA+主体尚不开源，Vodka 是VOFA+上位机的插件库（这个库是开源的），当前包含3个协议、5个控件。

![](http://henjay724.com/image/biweekly20210425/Vodka.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

