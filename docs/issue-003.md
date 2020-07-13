# 痞子衡嵌入式半月刊： 第 3 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 2 期》](https://www.cnblogs.com/henjay724/p/12326587.html)

## 唠两句

今天是雨水与惊蛰交节之时，惊蛰节气在农耕上有着相当重要的意义，自古以来我国人民很重视惊蛰这个节气，把它视为春耕开始的节令。

新冠肺炎疫情在逐日好转，相信大部分人都已经开始陆续复工了，但痞子衡东家还是决定 3 月 23 号之后再考虑全面复工的事。因此这些天痞子衡在家主要是以看技术文档写技术文档以及线上客户支持为主，最近原创文章产出比较惊人，一周能达到 3 篇，写文章这种事，写作过程中比较痛苦，但写完还是成就感满满的。

最近痞子衡不断接到技术群的朋友约稿，趁着在家办公的时机，痞子衡会加快写作，尽早完成大家的约稿。

本期共收录 3条资讯、4个项目、2个工具、1个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、面向音频/语音应用的恩智浦 i.MXRT600 已上市</font>

恩智浦半导体于 Embedded World 2020 上宣布其旗下主打音频/语音应用的全新跨界处理器 i.MXRT600 已开始正式供货，10K 量起价 $4.50，恩智浦官网上也逐渐放出了 i.MXRT600 相关开发资料。

i.MXRT600 特性如下：

```text
- 主频高达 300MHz 的Arm® Cortex®-M33内核
- 可选的Cadence® Tensilica® HiFi 4 音频、语音数字信号处理器（DSP）。运行主频高达 600MHz，并支持四组 32x32 MAC。
- 多达4.5MB 片上 SRAM，支持关键指令和数据的“零等待”访问。
- 28nm FD-SIO （耗尽型绝缘硅）工艺，提供更低的工作电流和漏电流。
- 内置恩智浦卓越的嵌入式安全技术 - EdgeLock™ 400A。
- 可使用 Glow 神经网络编译器，优化机器学习性能。
```

恩智浦除了提供常规软硬件开发工具支持外，还包括适用于 i.MXRT600 的 Cadence Xplorer IDE、DSP函数库和音频编解码器的支持。恩智浦还与 Alango Technologies、DSP Concepts 和 Sensory 合作，提供高性能语音预处理和识别软件以及专业的音频库和工具。

![](http://henjay724.com/image/biweekly/i.MXRT600_BlockDiagram.PNG)

### <font color="red">2、全球首颗通用 RISC-V MCU 兆易创新 GD32VF103 获 EW2020 唯一最佳硬件产品大奖 </font>

GD32VF103 是兆易创新（Gigadevice）于 2019 年 8 月 22 日发布的全球首款通用 RISC-V MCU，这款芯片日前获得了 Embedded World 2020 年度唯一的最佳硬件产品大奖。

GD32VF103 特性如下所示，其 Bumblebee 内核是由芯来科技（Nuclei System Technology）联合兆易创新针对其面向 IoT 或其他超低功耗场景的通用 MCU 产品定制的一款商用 RISC-V 处理器内核。

```text
- 提供108 MHz的运算主频，以及16~128 KB的片上闪存和6~32 KB的SRAM。
- 支持32比特宽的标准AHB-Lite系统总线接口，支持32比特宽的指令局部存储器。
- 支持32位的RISC-V指令集架构，支持RV32IMAC指令子集的组合。
- 主流支持标准JTAG接口 和RISC-V调试标准。
- 使用基于RISC-V的Bumblebee内核，该内核内置了单周期硬件乘法器、硬件除器。
```
兆易创新官方提供了两款 GD32VF103 开发板，一款是入门级 GD32VF103C-START，另一款是专业级 GD32VF103V-EVAL，下图便是专业级开发板：

![](http://henjay724.com/image/biweekly/GD32VF103V-EVAL.PNG)

### <font color="red">3、Micrium uC/OS 及其大部分组件推出免费商业授权(Apache License 2.0) </font>

Micrium 宣布于 2020 年 2 月底将 µC/OS-II, µC/OS-III, µC/FS, µC/TCP-IP, µC/USB-Device, µC/USB-Host, µC/CAN, µC/Modbus 转入 Apache License 2.0，客户可以免费商业使用。相关源码可在 SiliconLabs 官方 github 上获取：

```text
https://github.com/SiliconLabs/uC-OS2
https://github.com/SiliconLabs/uC-OS3
https://github.com/SiliconLabs/uC-FS
https://github.com/SiliconLabs/uC-TCP-IP
https://github.com/SiliconLabs/uC-USBD
https://github.com/SiliconLabs/uC-USBH
```

源于 1992 年的 uC/OS 应该是中国大部分嵌入式工程师的 RTOS 启蒙老师，除了其简单易用以及开源特性之外，邵贝贝老师翻译的 《嵌入式实时操作系统uC/OS-II》 对其推广也起了很大作用。

但是开源并不等于免费，早期的 uC/OS 仅可用于个人学习，如用作商业目的，Micrium 其实是要按产品出货量收费的。不过自从 2016 年 SiliconLabs 完成对 Micrium 的收购之后，uC/OS 逐渐放开商业授权，现在基本除了uC/GUI 之外，其它都可以免费商业使用了。

![](http://henjay724.com/image/biweekly/uCOS_Components.PNG)

## 项目类

### <font color="red">1、AMetal - 具有跨 MCU 平台通用接口的轻量级嵌入式开发平台</font>

AMetal 是周立功（ZLG）公司维护的芯片级裸机软件包，定义了跨平台的通用接口（使得基于 AMetal 的应用程序可以和具体硬件完全分离，实现跨平台复用），并提供了一系列驱动及常用的软件服务。AMetal 是周立功 AWorksOS 架构底层里的重要一环。

> 项目主页：http://www.zlgmcu.com/Category_2520/Index.aspx
> 代码主页：https://github.com/zlgopen/ametal

![](http://henjay724.com/image/biweekly/AMetal_Components.PNG)

AMetal 主要特点如下，其目前已经支持周立功、华大半导体、灵动微电子、恩智浦半导体等公司的 MCU 产品，并且其还支持了非常多的嵌入式里常用的驱动组件（见下表，未完全列出）

```text
- 将外设操作标准化，避免上层软件、驱动的再次开发；
- 能独立运行的软件包，全部开源，提供工程模板与DEMO程序，可在此基础上开发应用程序；
- 不依赖操作系统服务；
- 尽可能将外设的所有特性开放出来；
- 尽可能浅地对外设进行封装，把效率放在第一位；
- 用户不用看芯片手册也能使用。
```

![](http://henjay724.com/image/biweekly/AMetal_Device_list.PNG)

### <font color="red">2、TJpgDec - 为小型嵌入式系统高度优化的 JPEG 解码库</font>

TJpgDec 全称 Tiny JPEG Decompressor，是日本的大牛工程师 ChaN 开发的开源 JPEG 图像解码库（C代码），你可能对 ChaN 这个名字陌生，但我相信你对 ChaN 的另一个作品 FatFs 一定不陌生。

> 项目主页：http://elm-chan.org/fsw/tjpgd/00index.html

嵌入式项目里（尤其是视频相关）有时候经常需要跟 JPEG 格式打交道，关于 JPEG 解码最知名的莫过于 IJG 组织开发的 libjpeg 解码库，但是 libjpeg 主要针对 Linux 等大型 OS 平台开发的，而在嵌入式 MCU 平台下，TJpgDec 会更合适一点。

TJpgDec 特性如下，其极低的存储空间占用使其可以完美运行于小型 MCU，比如AVR, 8051, PIC, Z80, Cortex-M0 等。

```text
- Platform independent. Written in ANSI-C.
- Easy to use master mode operation.
- Fully re-entrant architecture.
- Very small memory footprint:
  - 3K bytes of RAM for work area independent of image dimensions.
  - 3.5-8.5K bytes of ROM for text and constants.
- Output format:
  - Scaling ratio: 1/1, 1/2, 1/4 or 1/8 selectable on decompression.
  - Pixel format: RGB888 or RGB565 pre-configurable.
```

![](http://henjay724.com/image/biweekly/TJpgDec.PNG)

### <font color="red">3、Micro:Boy - 基于微芯 ATtiny24 的简易电子游戏机</font>

这是来自 Hackaday 上的一个作品，基于 ATtiny24 和 MicroPython 的电子游戏机。

> 项目主页：https://hackaday.io/project/27757-microboy

![](http://henjay724.com/image/biweekly/ATtiny24_micro-boy_system.jpg)

> 游戏代码：https://hackaday.io/project/27757-microboy/log/78338-progress-on-a-game

![](http://henjay724.com/image/biweekly/ATtiny24_micro-boy_game.gif)

作者一开始想在 Micro:bit 平台上实现，但两个按键和 5x5 LED 最多只能做个贪吃蛇游戏。后来作者想到在 PewPew FeatherWing 平台上做，六个按键及 8x8 LED 能展示的余地大一些。不过最终作者还是选择了一个 ATtiny24 开发板以及 1.3" OLED SH1106 I²C 模块。

![](http://henjay724.com/image/biweekly/Micro-Bit_PewPew-FeatherWing.png)

### <font color="red">4、Metro M7 - 一款带 AirLift WiFi 模块的 i.MXRT1011 开发板</font>

Adafruit 网站上发现的一款带 AirLift WiFi 模块兼容 Arduino 的开发板，主控是恩智浦新推的 500MHz 主频的 i.MXRT1011，WiFi 模块是乐鑫的 ESP32，此板仍在研发中。

> 项目帖子：https://blog.adafruit.com/2020/02/29/metro-m7-rt1011-w-airlift-wifi-espressifsystem-nxp-arduino-adafruit/

![](http://henjay724.com/image/biweekly/Metro_M7_imxrt1011.PNG)

## 工具类

### <font color="red">1、RT-Thread Studio - RT-Thread 项目开发一站式工具(IDE)</font>

RT-Thread Studio 是 RT-Thread 团队于 2019 年 12 月 25 日全新推出的一站式开发工具，全面取代其上一代集成度不高的开发工具 ENV。

> 软件主页：https://www.rt-thread.org/page/studio.html

RT-Thread 是为数不多的国产 RTOS 之光，这些年的发展有目共睹，生态体系建设越来越完善，用户群也越来越庞大。RT-Thread Studio 就是其构建软件生态的重要一环。

RT-Thread Studio 主要包括工程创建和管理，代码编辑，SDK管理，RT-Thread配置，构建配置，调试配置，程序下载和调试等功能，结合图形化配置系统以及软件包和组件资源，减少重复工作，提高开发效率。

```text
- 社区版本永久免费
- 支持主流C/C++语言开发
- 强大的代码编辑和重构功能
- SDK管理器支持在线下载更新 RT-Thread 最新源码包
- 简单易用的工程创建向导，快速验证原型
- 全新图形化配置系统，同时支持架构图和树形图配置
- 软件包市场提供丰富的可用软件包资源
- 丰富的调试功能，快速查看和跟踪定位代码问题
```

![](http://henjay724.com/image/biweekly/RT-Thread_Studio.PNG)

### <font color="red">2、emWin AppWizard - 面向下一代嵌入式应用的 emWin 界面构建工具</font>

AppWizard 是 SEGGER 公司为其嵌入式 GUI 库 emWin 全新设计的面向下一代嵌入式应用的界面构建工具，伴随着 emWin v6.10 （2020年3月）一起发布，用于取代之前的界面构建工具 GUIBuilder。

> 产品主页：https://www.segger.com/products/user-interface/emwin/tools/tools-overview/#appwizard

emWin 是非常流行的嵌入式 GUI 库，界面构建一直是 GUI 开发中的痛点，SEGGER 于 emWin v5.10 时（2011年8月）开始推出的 GUIBuilder 工具一定程度上帮助用户减轻了 GUI 开发的工作量，但 GUIBuilder 诞生至今近 9 年里因其较弱的功能一直备受吐槽。如 GUIBuilder 只适合单窗口编辑，并且不支持汉字字体，窗体风格设计等。

![](http://henjay724.com/image/biweekly/emWin_GUIBuilder_rel.PNG)
![](http://henjay724.com/image/biweekly/emWin_GUIBuilder_ui.PNG)

一切爱恨，皆是过往，如今 AppWizard 来了，这是一个真正的所见即所得的界面构建工具，其典型功能如下：

```text
- Complete and ready-to-run emWin applications
- Support of emWin's core features such as widgets, animations and language management
- Resource management for fonts and bitmaps - Multilingual text management
- Application's behavior can be defined with interactions
- Integrated play mode makes testing simple
- Exportable to simulation or target project through included BSPs
- Little to no experience with emWin or even C required 
```

![](http://henjay724.com/image/biweekly/emWin_AppWizard_rel.PNG)
![](http://henjay724.com/image/biweekly/emWin_AppWizard_gui.PNG)

## i.MXRT出品

### <font color="red">1、谷歌 - Stadia 云游戏手柄</font>

Stadia 云游戏平台，可以使玩家们打破硬件性能和游玩地点的限制，仅仅通过网络就可以在 PC、平板电脑、手机等各种设备上体验到原汁原味的 3A 游戏大作。Stadia 手柄是这个云游戏平台的配套设备，其除了常规的按钮和操作杆之外，还有一个专用按钮用于截取屏幕和录制视频剪辑。

> RT芯片：i.MXRT1062
> 产品主页： https://www.stadia.dev/
> 官网定价： 69 美元起

![](http://henjay724.com/image/biweekly/Stadia_440x246.gif)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


