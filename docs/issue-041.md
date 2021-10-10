# 痞子衡嵌入式半月刊： 第 41 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 40 期》](https://www.cnblogs.com/henjay724/p/15315617.html)

## 唠两句

这周五是寒露，历史上的今天：1925年10月10日，北京故宫博物院首次对外开放。

本期共收录 4个项目、1个工具，希望对你有帮助！

## 项目类

### <font color="red">1、AliOS Things - 阿里出品轻量级物联网嵌入式操作系统</font>

AliOS Things 发布于2017年杭州云栖大会， 是 AliOS 家族旗下的、面向IoT领域的、高可伸缩的物联网操作系统。AliOS Things 致力于搭建云端一体化IoT基础设施，具备极致性能、极简开发、云端一体。

> 项目主页： https://github.com/alibaba/AliOS-Things

AliOS Things 支持多种CPU架构，包括：ARM，C-Sky，MIPS，RISCV等。AliOS Things 适配了分层架构和组件架构，包括下图全部组件，所有的模块都作为组件的形式存在，通过yaml进行配置，应用程序可以很方便的选择需要的组件。

![](http://henjay724.com/image/biweekly20211010/AliOS-Things.PNG)

### <font color="red">2、ECBM - 基于STC8系列的通用底层驱动函数库</font>

ECBM 是基于STC8单片机的外设函数库，也是“Everything Can Be Module”的简称，意思是“一切都可以成为模块”，其宗旨是“软件、硬件模块化，只造一次轮子”。目前该库已经演进到了V3版本，支持STC8全型号。库的作者是奈特，一枚6年STC铁粉。

> 项目主页： https://gitee.com/jackchio/ecbm_library

STC8是目前51单片机里最好用的系列，拥有最多8K的SRAM、64K的Flash、5个定时器、4个串口。全系列都带IIC和SPI，大部分带ADC。STC8H还带有硬件USB。

### <font color="red">3、stcgal - STC单片机的命令行编程工具</font>

stcgal 是 STC MCU 的命令行编程工具，兼容 8051 系列单片机。是 STC Windows 软件的全功能开源替代品，便携使用，适合自动化。

> 项目主页： https://github.com/grigorig/stcgal

功能特性包含：

```text
1. 支持 STC 89/90/10/11/12/15/8 系列
2. 支持 UART 和 USB BSL
3. 显示芯片信息
4. 确定的操作频率
5. 编程 flash
6. 编程 IAP/EEPROM
7. 设置设备选项
8. 读取唯一设备ID(STC 10/11/12/15/8)
9. 修整RC振荡器频率(STC 15/8)
10. 使用 DTR 切换或自定义 shell 命令自动重启电源
11. 自动的 UART 协议检测
```

### <font color="red">4、nRF51_Platform - 基于nRF51平台(蓝牙4.0)的轻量级SDK</font>

nRF51_Platform 是基于nRF51平台开发的一套轻量级SDK，可大大地降低低功耗蓝牙开发的门槛。

> 项目主页： https://github.com/JUMA-IO/nRF51_Platform

只要会C语言，就可以开发蓝牙硬件，因为SDK已经将所有蓝牙的通信配置，对于寄存器的处理步骤，封装在了一些简易识别的API中，用户只需要调用合适的api即可实现相应的功能，符合初学者的逻辑，不需要了解蓝牙协议栈的复杂名词和架构。

![](http://henjay724.com/image/biweekly20211010/nRF51_Platform.PNG)

## 工具类

### <font color="red">1、Mind+ - 图形化Arduino编程工具</font>

Mind+ 是一款开源的图形化Arduino编程工具，在Windows，Mac和Linux上都能运行。无需任何编程背景，只需拉拽选择模块，设定参数，给模块连线并上传到Arduino，便能轻松快速的完成模型。编程从未变得如此快速和简单。

> 工具主页： https://github.com/DFRobot/Mindplus-Desktop

![](http://henjay724.com/image/biweekly20211010/Mind+.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

