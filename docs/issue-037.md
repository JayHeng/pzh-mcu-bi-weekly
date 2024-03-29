# 痞子衡嵌入式半月刊： 第 37 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 36 期》](https://www.cnblogs.com/henjay724/p/15057813.html)

## 唠两句

昨天是立秋，历史上的今天：2008年8月8日，第29届夏季奥林匹克运动会在北京开幕。

本期共收录 2个资讯、4个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、TI 发布全新 Sitara™ AM2x 系列高性能MCU</font>

德州仪器 (TI) 近日推出了全新高性能微控制器产品系列 Sitara AM2x，推动了边缘端的实时控制、网络互联和智能分析。

> 资讯主页： https://e2e.ti.com/blogs_/b/process/posts/5-ways-high-performance-mcus-are-reshaping-the-industry

Sitara™ AM2x MCU产品系列基于高性能Arm® MCU内核，包含运行速度高达1 GHz的单核和多核器件，并集成了专用外设和加速器。AM243x MCU是首款可用的AM2x系列器件，具有多达四个Arm Cortex®-R5F内核，每个内核运行频率高达800MHz。

Sitara AM243x 器件扩展了 TI 对多个千兆工业以太网协议和时间敏感网络 (TSN) 的支持，可实现下一代工厂网络。借助 AM243x，工程师可以利用经过认证的、TI 直接提供的协议栈支持 EtherNet/IP™、EtherCAT®、PROFINET® 和 IO-Link 主站等，从而满足不断发展的工业通信标准。

![](http://henjay724.com/image/biweekly20210808/Sitara-AM2x.PNG)

### <font color="red">2、乐鑫发布 IEEE 802.15.4 + Bluetooth 5.2 (LE) RISC-V SoC ESP32-H2</font>

乐鑫科技近日宣布推出 ESP32-H2 芯片，首次在 2.4 GHz 频段集成 IEEE 802.15.4 和 Bluetooth 5.2 (LE) 技术。

> 资讯主页： https://www.espressif.com/zh-hans/news/ESP32_H2

ESP32-H2 搭载 RISC-V 32 位单核处理器，主频高达 96 MHz，内置 256 KB SRAM，并支持扩展外部 flash。ESP32-H2 融合了两种重要的无线连接技术：IEEE 802.15.4 针对低功耗 mesh 网络场景，通过对 Thread 和 Zigbee 协议的支持，使其拥有广阔的应用领域；Bluetooth LE 支持点对点、广播和 mesh 组网等多种拓扑结构，并能够与智能手机直接通信。

IEEE 802.15.4 和 Bluetooth LE 的结合，也将赋能 ESP32-H2 构建基于 Matter 协议的智能家居设备，实现多生态系统的互联互通。

![](http://henjay724.com/image/biweekly20210808/ESP32-H2.PNG)

## 项目类

### <font color="red">1、pyOCD - 用于调试烧写 Cortex-M 芯片的开源 Python 包</font>

pyOCD 是一个开源 Python 软件包，用于多种受支持的硬件调试器（DAP-Link、J-Link、ST-Link）下编程和调试Arm Cortex-M微控制器。它是完全跨平台的，并支持Linux，macOS和Windows。它内置支持多达70种流行的MCU。

> 项目主页： https://github.com/pyocd/pyOCD

pyOCD 允许用户通过命令来：烧录、擦除、单步、停止、设置断点、全速运行、芯片上锁、读写外设寄存器、读写存储空间等操作。

### <font color="red">2、CANable - 开源 USB 转 CAN 适配器</font>

CANable 是一个小型的低成本开源 USB-to-CAN 适配器。CANable在计算机上显示为虚拟串行端口，并充当到CAN总线接口的串行线。

> * 项目官网： https://canable.io/
> * 固件主页： https://github.com/candle-usb/candleLight_fw

CANable 与基于ARM的嵌入式平台兼容，如Raspberry Pi、Raspberry Pi Zero、ODROID、BeagleBone等，非常适合集成到OEM产品中。

![](http://henjay724.com/image/biweekly20210808/CANable_v2.PNG)

### <font color="red">3、Cumu - 开源智能 WIFI 万用表</font>

Cumu 是 elecfans 坛友设计的一台智能 WIFI 万用表，主控是 STM32F030，万用表芯片采用 FS9721，整体硬件成本在100元左右。它具有物联网功能，你身边所有的智能设备都将是这台万用表的显示窗口。  

> 项目介绍： https://bbs.elecfans.com/jishu_489788_1_1.html

Cumu 支持乐联网、YEELINK和传感云免费物联网平台，可以将测量数据上传到平台上，平台有很多玩法，比如：设置上下限、短信报警、微信获取数据等，Cumu的使用范围很广阔。

![](http://henjay724.com/image/biweekly20210808/Cumu.PNG)

### <font color="red">4、thundercracker - sifteo二代智能积木开源软件工具链</font>

Sifteo 是 david merrill 博士设计的一个基于 STM32 和 nRF24LE1 微控制器无线网络的有形视频游戏系统，这个产品也在2011的CES上获得了创新奖。很可惜公司于2014年被当时正在风口的北美最大的消费无人机公司3DR收购，sifteo的工程团队也就都转做无人机。  

> * 项目介绍： https://blog.adafruit.com/2012/12/05/how-we-built-a-super-nintendo-out-of-a-wireless-keyboard-sifteo-sifteo
> * 项目主页： https://github.com/sifteo/thundercracker

thundercracker 是 Sifteo 软件工具链，现如今全部开源了，通过这个库我们可以学习到如下知识：

```text
a. C/C++、lua、Makefile等语言
b. STM32/24LE1单片机学习、STM32、USB升级、swiss
c. 24LE1/24L01无线传输
d. 游戏制作
e. STM32模拟器
f. doxgen生成源码文档
```

![](http://henjay724.com/image/biweekly20210808/thundercracker-cube51sim.gif)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

