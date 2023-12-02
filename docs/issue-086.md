# 痞子衡嵌入式半月刊： 第 86 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 85 期》](https://www.cnblogs.com/henjay724/p/17826449.html)

## 唠两句

历史上的今天：1942年12月2日，在意大利物理学家费米的主持下，美国建立了世界上第一座原子反应堆。

本期共收录 1 个资讯、4 个项目、1 个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、Arm Cortex-M52发布，将人工智能引入超小型端点设备</font>

近日 ARM 宣布推出专为人工智能物联网 (AIoT) 应用而设计的 Arm® Cortex®-M52 处理器，Cortex-M52 处理器是支持 Arm Helium 技术中体积最小、面积与成本效益最好的产品，无需独立单元即可提供DSP功能（数字信号处理），有助于节省面积和成本，并提供可扩展的弹性以足各种性能与配置需求。

 * 资讯来源：https://newsroom.arm.com/news/arm-cortex-m52

Cortex-M52 采用与 Cortex-M55、Cortex-M85 相同的 Armv8.1-M架构，并支持Helium 矢量扩展方案（M-Profile Vector Extension，MVE），能够有效提高 ML（机器学习）与 DSP 应用的性能表现。与前代 Cortex-M33 相比，Cortex-M52 的 ML 性能提升 5.6 倍，DSP 性能则提升 2.7 倍。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-086/cortex-m52.PNG)

## 项目类

### <font color="red">1、emRun - Embedded Studio下C/C++标准库</font>

emRun 是 SEGGER 对大多数 GCC 工具链中使用的 newlib、newlib-nano 和 glibc 的替代品。与用于嵌入式系统的专业运行时库相比，这些库有明显的缺点。emRun 将任何基于 gcc 的工具链转换为专业的开发选择。

 * 项目地址：https://www.segger.com/products/development-tools/runtime-library/

在许多情况下，emRun 节省的 rom 可以使用更小的微控制器和更少的片上内存。这可以大大节省成本，特别是对于为大众市场大量生产的设备。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-086/emRun.PNG)

### <font color="red">2、cpost - C语言程序上下文切换和解耦</font>

cpost 是一个 C 语言编写的，用于 C 语言程序上下文切换和解耦的工具。cpost 包含 cpost 和 cevent 两个工具，cpost 用于 C 语言的上下文切换，cevent 用于程序模块之间的解耦。

 * 项目地址：https://github.com/NevermindZZT/cpost

cpos t借鉴了 Android 的 Handler 机制，在 C 语言环境中，可以通过调用 cpost 接口，将函数抛出到另外的线程(上下文)中运行，对于某些场景，尤其是嵌入式编程无操作系统环境下的中断延迟处理。

cevent 借鉴了 Android 的广播机制，在 C 语言环境中，当程序运行至相应的位置，可以通过 cevent 接口抛出一个事件，其他模块可以通过注册的方式，监听这个事件，当事件发生时，调用注册的函数，能很大程度上实现模块间的解耦。 

### <font color="red">3、Magnetic_Rotary_Encoding - 高分辨率磁旋转编码库</font>

Magnetic_Rotary_Encoding 是一个用于在 C/C++ 和 MicroPython 中设置磁旋转编码的库，该库还具有一个触觉控制器，允许用户连接和控制振动电机作为步长计数触觉反馈。

 * 项目地址：https://github.com/ahmsville/Magnetic_rotary_encoding

该库一共有三种硬件版本，下图是其一，这是一个完全成熟的开发板与磁性旋转编码器相结合，它是用树莓派 RP2040 微控制器芯片构建的，基本分辨率为 36，可扩展到每转 36000 步。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-086/Magnetic_Rotary_Encoding.PNG)

### <font color="red">4、jellyfish-and-starfish - 用于电子元件拾取放置的电机控制板</font>

Starfish 是一个基于树莓派 RP2040 微控制器和 Trinamic TMC2209 电机驱动器构建的拾取和放置机的控制板。这个控制板与 3D 打印机控制板有一些相似之处，但它有一些独特的问题需要解决——包括控制螺线管和与真空传感器交互。

 * 项目地址：https://github.com/wntrblm/jellyfish-and-starfish

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-086/starfish.PNG)

## 工具类

### <font color="red">1、LibrePCB - 免费的跨平台 EDA</font>

LibrePCB 是一款免费的跨平台电子设计自动化套件，用于创建原理图和设计印刷电路板。它专为各种技能水平的创客、学生和专业人士而设计。

 * 工具地址：https://librepcb.org/

LibrePCB 易于学习和使用，具有简单直观的用户界面。它提供了智能库概念、干净的文件格式以及无缝安装库和订购 PCB 的能力。LibrePCB 还支持任务自动化，是一款根据 GPLv3 授权的开源软件。  

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-086/LibrePCB.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

