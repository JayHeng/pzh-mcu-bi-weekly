# 痞子衡嵌入式半月刊： 第 79 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 78 期》](https://www.cnblogs.com/henjay724/p/17512804.html)

## 唠两句

历史上的今天：1923年7月30日，中国自行设计生产的第一架双层螺旋桨敞盖飞机由广东飞机制造厂研制成功命名为“洛士文一号”。

本期共收录 4 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、RTIC - 基于RUST的开源免费实时中断驱动系统</font>

RTIC 是 Real-Time Interrupt-driven Concurrency 缩写。从 RTIC 开发商的角度看，RTIC是一种硬件加速的 RTOS，它利用 Cortex-M mcu 中的 NVIC 来执行调度，而不是更经典的软件内核。来自社区的另一个常见观点是，RTIC 是一个并发框架，因为它没有软件内核，而且依赖于外部 hal。

> * 项目地址：https://github.com/rtic-rs/rtic

RTIC 特性包括：

```text
- 任务作为并发单位1。任务可以由事件触发(响应异步刺激而触发)，也可以由应用程序按需生成。
- 任务之间的消息传递。具体来说，消息可以在生成时传递给软件任务。
- 一个定时器队列。软件任务可以安排在将来某个时间运行。该特性可用于实现周期性任务。
- 支持任务的优先级，因此，抢占式多任务。
- 通过基于细粒度优先级的临界区实现高效且无数据竞争的内存共享。
- 在编译时保证无死锁执行。这是比标准互斥锁抽象提供的更强的保证。
- 最小的调度开销。任务调度程序具有最小的软件占用;硬件完成了大部分的调度。
- 高效的内存使用:所有任务共享一个调用堆栈，并且没有对动态内存分配器的硬依赖。
- 完全支持所有Cortex-M设备。
- 此任务模型适用于已知的WCET(最坏情况执行时间)分析和调度分析技术。
```

### <font color="red">2、ETL - 嵌入式C++模板库</font>

C++是用于嵌入式应用程序的优秀语言，模板是一个强大的方面。本项目 Embedded Template Library (ETL) 不是为了完全取代 STL 而设计的，而是对它的补充。

ETL 是为低资源的嵌入式应用而设计的。它包含一组容器、算法和实用程序，其中一些模拟了 STL 的一部分。没有动态内存分配。库不使用堆。所有容器都有一个固定的容量，允许在编译时确定所有内存分配。

> * 项目地址：https://github.com/ETLCPP/etl

### <font color="red">3、STM32 Emulator - 基于STM32的3D打印机模拟器</font>

这个项目的目标是模拟3D打印机，适用于任何类型的 stm32 微控制器固件，STM32 硬件外设全部采用模拟的方式实现。这个模拟器是在作者对逆向工程3D打印机的工作背景下完成的。

> * 项目地址：https://github.com/nviennot/stm32-emulator

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-079/STM32-Emulator.gif)

### <font color="red">4、FlipDigits - 用于在7段数码管显示器上渲染图形的处理应用程序</font>

FlipDigits 是一个开源的处理应用程序，可以在7段数码管显示器上运行图形，该项目基于的显示器是由448个7段数字组成的机械翻转数字显示器。

> * 项目地址：https://github.com/owenmcateer/FlipDigits

作者为了实现各种炫酷效果展示，专门设计了配套上位机：

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-079/FlipDigit-UI.gif)

## 工具类

### <font color="red">1、2bit-Video-Processor - 二值视频格式转换工具</font>

这是一个小程序，将视频图像序列转换为用于2bit显示器(如FlipDots)的原始数据文件。2位意味着两种单色或开/关，没有灰度和alpha。适合用在单色屏上，比如OLED这些。

> * 项目地址：https://github.com/owenmcateer/2bit-Video-Processor

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-079/2bit-Video-Processor.PNG)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-079/2bit-Video-Processor.gif)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

