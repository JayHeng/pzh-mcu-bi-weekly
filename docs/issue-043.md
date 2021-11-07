# 痞子衡嵌入式半月刊： 第 43 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 42 期》](https://www.cnblogs.com/henjay724/p/15418226.html)

## 唠两句

今天是立冬，历史上的今天：2000年11月7日，周杰伦第一张同名专辑《Jay》发布。

本期共收录 2个资讯、3个项目、1个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、平头哥发布自研云芯片倚天710</font>

2021云栖大会现场，阿里巴巴旗下半导体公司平头哥发布自研云芯片倚天710。

倚天710采用业界最先进的5nm工艺，单芯片容纳高达600亿晶体管；在芯片架构上，基于最新的ARMv9架构，内含128核CPU，主频最高达到3.2GHz，能同时兼顾性能和功耗。

为解决云计算高并发条件下的带宽瓶颈，倚天710针对片上互联进行了特殊优化设计，通过全新的流控算法，有效缓解系统拥塞，从而提升了系统效率和扩展性。在标准测试集SPECint2017上，倚天710的分数达到440，超出超过业界标杆20%，能效比提升50%以上。

![](http://henjay724.com/image/biweekly20211107/t-head_yitian710.PNG)

### <font color="red">2、中国首款宇航级存储控制器芯片Bifort</font>

Bifort 是西安艾可萨科技推出的适用于宇航应用的PCIe Gen2x4 / SATA3双接口SSD控制器。

Bifort是一个高性能，高可靠性 PCIe/SATA双接口控制器，同时提供了防辐射加固以防止恶劣的太空环境所造成的辐照总剂量效应、单粒子翻转效应、单粒子闩锁效应，为宇航应用构建高容量SSD提供完美的解决方案。

Bifort可以提供PCIe Gen2x4 / SATA3主控接口，并提供6个独立的Flash 通道，控制器配备两个RISC CPU 以达到杰出的性能。

> * 产品主页：https://www.exadevice.com/productinfo/30319.html

![](http://henjay724.com/image/biweekly20211107/Bifort.PNG)

## 项目类

### <font color="red">1、OpenOCD - 开源的片上调试器（GDB服务程序）</font>

OpenOCD（Open On-Chip Debugger）是一个开源的片上调试器，它可以控制包括Wiggler之内的很多JTAG硬件，我们可以将它理解为一种GDB服务程序。OpenOCD 旨在提供针对嵌入式设备的调试、系统编程和边界扫描功能。

> * 项目官网：https://openocd.org/
> * 项目主页：https://github.com/openocd-org/openocd

OpenOCD 的功能需要调试仿真器来辅助完成，调试仿真器是一个提供调试目标电信号的小型硬件单元。常用的有JLink、STLink等，一些开发板直接集成了调试仿真器。

下面的 OpenOCD 架构图可以看出 OpenOCD 提供了GDB Server，可以通过它进行GDB相关的调试操作。提供Telnet Server，可以通过Telnet连接对目标板进行烧录、重启等操作。OpenOCD的配置基于TCL脚本，可以使用默认自带的TCL脚本，也可以编写自定义的脚本。

![](http://henjay724.com/image/biweekly20211107/OpenOCD.PNG)

### <font color="red">2、Mega-Cube - 4096个RGB LED的光立方（16x16x16）</font>

Mega-Cube 是一个基于 PL9823 驱动 4096 个 LED 的光立方，主控方面是基于恩智浦 i.MXRT1060 FlexIO 功能的Teensy4.0 和很多个 595 移位寄存器，最多能控制32个通道，每个通道1000个LED。

> * 项目主页：https://github.com/MaltWhiskey/Mega-Cube

i.MXRT1060 中带有DMA功能的FlexIO，每秒能驱动100万个LED的更新，大概算下来，32个通道，每个通道100个LED以330帧/秒的速度更新，这还是没有CPU干预的情况下，这样可以带一个屏幕，同步显示光立方上面的运行动画。

![](http://henjay724.com/image/biweekly20211107/Mega-Cube2.PNG)

![](http://henjay724.com/image/biweekly20211107/Mega-Cube.PNG)

### <font color="red">3、soft-and-hard - 基于JS的经典入门物联网教程</font>

soft-and-hard 是一个以物联网项目为主方向分享 web 开发教程，制作并演示一个物联网系统是怎么跑起来的，介绍如何学习相关知识。

> * 项目主页：https://github.com/alwxkxk/soft-and-hard

教程内容包括：

```text
1. 硬件上选择价格便宜(淘宝价十几块钱)的NodeMCU开发板，使用Arduino进行开发。
2. 物联网你还得先懂网，在教程中简单介绍了计算机网络基础知识、TCP/IP协议、HTTP协议、MQTT协议等等。
3. Web上选择了无所不能的JavaScript，在教程中将会演示其在网页开发、小程序开发、桌面应用开发、服务器后端服务开发。
4. 整个教程里，推荐先用后学，先把项目跑起来看看效果，再按需学习相关知识，直到自己能把项目写出来。
```

demo1演示了最简的系统，实现软件显示硬件的数据，可控制硬件执行动作。 

![](http://henjay724.com/image/biweekly20211107/soft-and-hard1.jpg)

在demo1的基础上，demo2添加了MongoDB数据库、实时显示数据（websocket协议）、数据可视化(Echart图表)功能。 

![](http://henjay724.com/image/biweekly20211107/soft-and-hard2.jpg)

## 工具类

### <font color="red">1、gdbgui - gdb调试的一个Web可视化扩展</font>

gdbgui 是gdb的一个Web可视化扩展，可以向开发人员提供Web展示前端，因此可以在浏览器中实现断点添加，堆栈查看跟踪以及更改上下文和参数值等操作。

> * 软件官网：https://www.gdbgui.com/
> * 软件主页：https://github.com/cs01/gdbgui

![](http://henjay724.com/image/biweekly20211107/gdbgui.gif)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

