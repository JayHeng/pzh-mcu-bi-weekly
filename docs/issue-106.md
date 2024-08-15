# 痞子衡嵌入式半月刊： 第 106 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 105 期》](https://www.cnblogs.com/henjay724/p/18314326)

## 唠两句

历史上的今天：1997年8月15，Linux平台上主流的桌面环境GNOME创始人 Miguel de Icaza 通过电子邮件宣布GNOME问世。

本期共 4 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、Grbl - 开源嵌入式G代码解析器</font>

Grbl 是一个高性能，低成本的以并行端口为基础的 CNC 运动控制器固件。它可以运行在 Arduino (Duemillanove/Uno) 上。控制器是用高度优化的 C 语言编写的，利用 avr 芯片的外设功能来实现精确的定时和异步操作。它能够保持高达 30kHz 的稳定，无抖动控制脉冲。

Grbl 接受符合标准的 G 代码，并已与几个 CAM 工具的输出进行了测试。弧，圆和螺旋运动完全支持，以及所有其他主要的 G 代码命令。

 * 项目地址：https://github.com/grbl/grbl

### <font color="red">2、grblHAL - 可定制的CNC控制器解决方案</font>

grblHAL 是针对 32 位处理器的 Grbl v1.1 的重写版。引入硬件抽象层(HAL)是为了将核心 Grbl 代码与处理器/硬件特定代码(驱动编码器)完全分离。驱动程序代码通过函数指针从核心访问，驱动程序通过 HAL 结构中的这些和标志宣布实现的功能。

目前有超过 13 种处理器（包含 RT1062、STM32F4、RP2040、LPC1700 等）驱动程序可供使用，这些驱动程序的功能取决于可用资源，如 GPIO 引脚数量和处理器外设。驱动程序通过HAL结构“告诉”内核什么是可用的，内核相应地调整自己。编写额外的驱动程序相对容易，因为不需要对核心进行修改——驱动程序可以在单个单独的文件中实现。

 * 项目地址：https://github.com/grblHAL

 ### <font color="red">3、PicoCNC - 4轴CNC运动控制器</font>

PicoCNC 是一个控制子板，可与 grblHAL 和 Rapsberry Pi Pico 微控制器一起，为路由器、铣床、激光和车床等设备创建了一个强大的 CNC 运动控制器。软件基于 grblHAL，它构成了具有先进功能的运动控制系统的基础。

 * 项目地址：https://github.com/phil-barrett/PicoCNC/

PicoCNC 特性包括：

```text
- 通过螺钉端子和销头支持多达4轴
- 主轴控制：PWM (5 v)、方向(5 v)、0-10V、支持12V PWM(通过开路集电极输出)
- 每个轴增加限位开关
- 包含继电器的支持
- 隔离标准Grbl输入控制: 循环启动，饲料保持，停止和安全门
- 光隔离探头输入
```

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-106/PicoCNC.PNG)

### <font color="red">4、linux-ch32v003 - 在ch32v003单片机上运行Linux</font>

这个项目实现了在 CH32V003 微控制器上运行 Linux 操作系统。它通过使用一个 8MB 的 SPI PSRAM 芯片和一个 RISC-V 模拟器(mini-rv32ima)来实现这一点。模拟器是必需的，因为 PSRAM 不能映射到微控制器的地址空间。Linux 内核和 rootfs 在引导时从 SD 卡加载到 PSRAM 中，文件系统基于 FatFs 库。

 * 项目地址：https://github.com/tvlad1234/linux-ch32v003

## 工具类

### <font color="red">1、exe_to_dll - 将EXE转换为DLL的小工具</font>

这个小工具可以转换 EXE，以便它可以像 DLL 一样加载。工具支持 32 位和 64 位 DLL。

 * 工具地址：https://github.com/hasherezade/exe_to_dll

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-106/exe_to_dll.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

