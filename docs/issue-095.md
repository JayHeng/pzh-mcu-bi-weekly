# 痞子衡嵌入式半月刊： 第 95 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 94 期》](https://www.cnblogs.com/henjay724/p/18064655)

## 唠两句

历史上的今天：1950年3月17日，美国加州伯克利大学发现第98号元素锎(Cf, californium)。

本期共收录 2 个资讯、2 个项目、1 个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、意法半导体推出600MHz主频的STM32H7R/S</font>

近日，意法半导体发布了一款新的集MPU和MCU两者之长的高性能产品 STM32H7R/S，搭载了在意法半导体迄今发布的产品中性能最高的Arm®Cortex®-M内核(最高运行频率600MHz的Cortex-M7。新微控制器具有强大的安全功能，能够满足物联网(IoT)应用对网络安全的要求。两款产品的共同安全功能包括防止物理攻击、存储器保护、在运行时保护应用程序的代码隔离保护功能，以及平台验证。此外，STM32H7S产品还增加了更多的强化的安全功能，集成了不可变的信任根、调试验证，以及硬件加密加速器，其中，硬件加密加速器支持最新的加密算法，防止非法访问代码和数据。利用这些安全保护功能，这两款产品聚焦于SESIP3和PSA 3级以下安全认证，满足业内最高的网络安全保护标准。

 * 资讯来源：https://newsroom.st.com/zh/media-center/press-item.html/p4615.html

新产品细分为两个产品线：STM32H7R3/S3 通用MCU和图形处理能力增强的 STM32H7R7/S7。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-095/STM32H7RS.PNG)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-095/STM32H7RS-2.PNG)

### <font color="red">2、先楫半导体推出面向数字仪表显示及人机界面应用的HPM6800</font>

近日，先楫半导体推出了新一代数字仪表显示及人机界面系统应用平台——HPM6800系列。该系列产品结合主频600MHz RISC-V CPU内核，算力高达1710DMIPS，采用了芯原的高性能2.5D OpenVG GPU，支持OpenVG Lite图形库和2D图形加速PDMA，内置1MB RAM，支持DDR2/DDR3/DDR3L接口，集成2组 4 Lane MIPI-DSI/LVDS-Tx 显示接口和2组 2 Lane MIPI-CSI/LVDS-Rx 摄像头接口，单芯片MCU开发简便，启动时间低至百毫秒，系统功耗低，赋予数字仪表显示和人机界面应用巨大的发展潜力。

 * 资讯来源：http://www.hpmicro.com/product/series.html?id=0710b474-83e2-47b9-8631-784fa60a49bb

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-095/hpm6800.png)

## 项目类

### <font color="red">1、qmk_firmware - 一个开源的键盘固件</font>

qmk_firmware 是一个开源的键盘固件，适用于 Atmel AVR 和 Arm USB 系列芯片，包括了一系列开源键盘项目和固件代码。它由来自开源社区的程序员和键盘爱好者共同维护和开发，旨在为用户提供高度可定制的键盘体验。

 * 项目地址：https://github.com/qmk/qmk_firmware

qmk_firmware 功能和特点：

```text
• 灵活的键盘布局和映射：qmk_firmware允许用户自定义键盘布局，可以在一个键盘上使用多种布局，并通过编程映射按键功能。这为用户提供了极大的灵活性和便利性，满足个性化设置和定制需求。
• 丰富的功能支持：qmk_firmware提供了丰富的功能支持，包括多种按键动作（单击、双击、长按等）、多层按键、宏、媒体控制、RGB背光控制等。用户可以根据自己的需求实现各种独特的功能和效果。
• 跨平台兼容性：qmk_firmware支持多种操作系统，包括Windows、Mac和Linux。这使得用户可以在不同的机器上进行键盘定制和编程，无论是个人电脑还是嵌入式系统。
• 活跃的开源社区：作为一个开源项目，qmk_firmware拥有活跃的社区支持。用户可以在论坛、GitHub和社交媒体上与其他开发者和用户交流思想、分享自己的项目和成果，从中获取技术支持和灵感。
```

### <font color="red">2、FabGL - 一个面向ESP32的图形库</font>

FabGL 主要是 ESP32 的图形库。它实现了几个显示驱动程序(用于直接VGA输出和I2C和SPI LCD驱动程序)。FabGL 也可以从 PS/2 键盘和鼠标获得输入。ULP 核心处理 PS/2 端口通信，使主 CPU 核心自由执行其他任务。FabGL 还实现:一个音频引擎，一个图形用户界面(GUI)，一个游戏引擎和一个 ANSI/VT 终端。

 * 项目地址：https://github.com/fdivitto/FabGL

## 工具类

### <font color="red">1、LVGLBuilder - 一个开源的LVGL界面编辑器</font>

LVGLBuilder 是一款强大而简便的 UI 界面设计工具，通过可视化的方式帮助开发者快速创建令人惊艳的用户界面。无论是初学者还是有经验的开发者，都可以轻松使用 LVGLBuilder 实现自己的创意和项目需求，省去繁琐的手动编码步骤。

 * 工具地址：https://github.com/CURTLab/LVGLBuilder

LVGLBuilder 支持多种嵌入式平台，包括但不限于 Arduino、ESP32、Raspberry Pi 等。这使得开发者能够在各种不同的硬件平台上使用 LVGLBuilder，实现跨平台开发，方便快捷地构建出精美的 UI 界面。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-095/LVGLBuilder.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

