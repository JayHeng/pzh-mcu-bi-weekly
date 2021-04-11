# 痞子衡嵌入式半月刊： 第 29 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 28 期》](https://www.cnblogs.com/henjay724/p/14590445.html)

## 唠两句

清明是上周日的事，历史上的今天：1910年4月11日津浦铁路（京沪铁路前身）首次开通旅客列车。

本期共收录 2条资讯、4个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、ARM推出了全新的Armv9架构</font>

近日，ARM推出了全新的Armv9架构，这是自Armv8十年前推出后，该架构首次重大变革。Armv9架构将会给接下来两代芯片带来30%的性能提升。

> 资讯主页: https://www.arm.com/company/news/2021/03/arms-answer-to-the-future-of-ai-armv9-architecture

![](http://henjay724.com/image/biweekly20210411/Armv9.PNG)

Armv9在兼容Armv8的基础上，提升了安全性、增强了矢量计算、机器学习及数字信号处理，同时继续提升处理器性能。

Armv9架构的处理器平衡了通用计算设备与处理数字信号和机器学习等任务的专用处理器的经济性、设计自由性和可访问性优势三方面。

### <font color="red">2、乐鑫发布新款RISC-V SoC ESP32-C6</font>

近日，乐鑫科技宣布推出 ESP32-C 系列中的又一款新品 ESP32-C6。ESP32-C6 是乐鑫首款集成 Wi-Fi 6 + Bluetooth 5 (LE) 的 32 位 RISC-V SoC，具有极低功耗和高性价比，能够大幅提升物联网设备的 Wi-Fi 传输效率，提供安全可靠的连接性能。

ESP32-C6 的 CPU、内存和安全性能与 ESP32-C3 相似，它搭载 RISC-V 32 位单核处理器，时钟频率高达 160 MHz，内置 400 KB SRAM，384 KB ROM，并支持多个外部 SPI、Dual SPI、Quad SPI、QPI flash。

> 资讯主页: https://www.espressif.com/zh-hans/node/5088

![](http://henjay724.com/image/biweekly20210411/ESP32-C6.PNG)

## 项目类

### <font color="red">1、Arm-2D - 基于Cortex-M的2D图形加速库</font>

ARM官方出品的2D图形加速库，在Cortex-M55系统频率 8MHz 下就可以实现30fps的渲染（6图层。320x240,rgb565）。

> 项目主页: https://github.com/ARM-software/EndpointAI/tree/master/Kernels/Research/Arm-2D

![](http://henjay724.com/image/biweekly20210411/Arm-2D_Alpha-blending.gif)

Arm-2D 库特性包括但不限于:

```text
* Alpha-Blending
    - With or without Colour-Masking
* Image Copy / Texture Paving
    - With or without Colour-Masking
    - Four mirroring mode: None, X-mirroring, Y-mirroring and XY-mirroring
* Colour format conversions
    - RGB565 and RGB888
    - Generic RGB16 and RGB32
* Region/Window Clipping
* Generic Partial Frame-buffer (PFB) Support
    - Transparent for upper layer software/GUI services
    - Easy to implement
    - No limitation on target screen resolution
    - No limitation on PFB size and shape (it could be line or cube with any size)
* Unified and User Friendly Programmers' Mode
    - APIs could be used in Synchronous manner ( Classic Blocking code ) and/or Asynchronous manner ( Event-Driven )
    - Support both bare-metal and RTOS
    - Ultra small memory footprint
```

![](http://henjay724.com/image/biweekly20210411/Arm-2D.PNG)

### <font color="red">2、ELL-8051-LIB - 面向8051的高效低封装函数库</font>

8051 ELL函数库，是网友泽文i针对STC8系列丰富的芯片资源，基于keil开发的软件包。函数库采用了LL库的编程思想，充分考虑8051的特性，结合硬件条件，提供大量标准的API函数，供开发者访问底层硬件细节。并且函数库的大小可裁剪，在代码密度和执行效率上做了很好的平衡。

> 项目主页: https://gitee.com/zeweni/ELL-8051-LIB

![](http://henjay724.com/image/biweekly20210411/ELL-8051-LIB.PNG)

### <font color="red">3、KLite - 简洁易用的嵌入式操作系统内核</font>

KLite是由个人编写的嵌入式操作系统内核，它是一款入门级的小型抢占式操作系统内核，以简洁易用为设计目标，旨在降低学习嵌入式操作系统编程和入门的难度。

> 项目主页: https://gitee.com/kerndev/klite

KLite 以其简洁的API风格，简洁的调用方式，简单的移植方法，可以算得上是目前最简单易用的嵌入式操作系统内核。

```text
-- 支持优先级抢占  
-- 支持相同优先级的线程  
-- 支持线程同步互斥  
-- 支持动态内存管理
-- 支持多编译器GCC, IAR, MDK
```

KLite 目前已经为ARM Cortex-M0/M3/M4做好了底层适配，如果你的CPU平台是基于以下平台：STM32,GD32,NRF51,NRF52,Freescale K40等系列单片机，那么可以直接使用预编译的库文件进行开发，只需要修改template.c里面几个简单的函数即可开始编程。

### <font color="red">4、LW_OOPC - 一种轻量级的面向对象的C语言编程框架</font>

LW_OOPC 是Light-Weight Object-Oriented Programming in(with) C的缩写, 这个框架是由台湾的高焕堂先生以及他的MISOO团队首创, 之后由金永华继续改进优化。

网友 Akagi201 在金永华对于高焕堂的lw_oopc的源码的基础上进行了一些简单的修改和调试，使得lw_oopc能够用在实际的嵌入式项目中, 作为一个很好的框架传播开来。

> 项目主页: https://github.com/Akagi201/lw_oopc

LW_OOPC 非常的轻量级, 但却很好的支持了很多面向对象的特性, 比如继承, 多态，可以优美的实现面向接口编程。

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

