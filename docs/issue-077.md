# 痞子衡嵌入式半月刊： 第 77 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 76 期》](https://www.cnblogs.com/henjay724/p/17365735.html)

## 唠两句

历史上的今天：1959年5月28日，美国将两只猴子（罗猴艾布尔和鼠猴贝克）载入“朱庇特号”火箭发射入太空，在火箭回收时猴子安然无恙。

本期共收录 4 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、Open-CMSIS-Pack - 简化物联网工作流和生命周期管理框架</font>

Open-CMSIS-Pack 项目将提供集成和管理软件组件的基础设施，并改善嵌入式和物联网项目之间的代码重用。该项目目前作为一个孵化项目由Linaro与Arm、NXP和ST合作主持和管理。

组件重用的软件兼容性长期以来一直是微控制器领域的一个挑战，特别是对于物联网来说，与PC或数据中心相比，物联网在硬件层面上更加多样化。Open-CMSIS-Pack将消除这种复杂性，为软件组件打包提供一个标准，并为验证、分发、集成、管理和维护提供相关的基础工具。

> * 项目地址：https://www.open-cmsis-pack.org/

### <font color="red">2、Secure Provisioning SDK - 面向NXP MCU的安全下载操作SDK</font>

SPSDK 是一个统一的、可靠的、易于使用的 Python SDK 库，可在 NXP MCU 产品组合中工作，为快速的客户原型设计到生产部署提供坚实的基础。该库允许用户与设备进行连接和通信、配置设备、准备、下载和上传数据，包括安全操作。

> * 项目地址：https://github.com/NXPmicro/spsdk

![](http://henjay724.com/image/biweekly20230528/SPSDK.PNG)

SPSDK 以以下形式交付:

```text
应用程序 - 可以使用Python虚拟环境从命令行调用的应用程序;
api - Python库形式的函数。
```

### <font color="red">3、ToolKit - 一套应用于嵌入式系统的通用工具包</font>

ToolKit 是一套应用于嵌入式系统的通用工具包，可灵活应用到有无RTOS的程序中，采用C语言面向对象的思路实现各个功能，尽可能最大化的复用代码，目前为止工具包包含：循环队列、软件定时器、事件集。

> * 项目地址：https://github.com/cproape/toolkit

```text
-Queue 循环队列
    1.支持动态、静态方式进行队列的创建与删除。
    2.可独立配置缓冲区大小。
    3.支持数据最新保持功能，当配置此模式并且缓冲区已满，若有新的数据存入，将会移除最早数据，并保持缓冲区已满。
-Timer 软件定时器
    1.支持动态、静态方式进行定时器的创建与删除。
    2.支持循环、单次模式。
    3.可配置有无超时回调函数。
    4.可配置定时器工作在周期或间隔模式。
    5.使用双向链表，超时统一管理，不会因为增加定时器而增加超时判断代码。
-Event 事件集
    1.支持动态、静态方式进行事件集的创建与删除。
    2.每个事件最大支持32个标志位。
    3.事件的触发可配置为**“标志与”和“标志或”**。
```

### <font color="red">4、tftpserver - 超简洁的tftp server</font>

TFTP（Trivial File Transfer Protocol，简单文件传输协议），基于 UDP 实现，提供不复杂、开销不大的文件传输服务，端口号为 69。常见的 tftp server 是 tftp-hpa，但其配置起来不是特别方便。

tftpserver 是一个超简单的 tftp server，C 语言编写，源码仅一个 532 行的 .c 文件，无任何依赖，开箱即用。

> * 项目地址：https://github.com/crossbowerbt/tftpserver

## 工具类

### <font color="red">1、serialporttool - 精品工控软件工具</font>

该公司出品的每个软件工具都是工控精品。自2003年以来，他们一直致力于串口和网络通信软件的开发。这家公司不仅提供软件产品，还提供定制和咨询服务。

> * 工具官网：https://www.serialporttool.com/GK/

![](http://henjay724.com/image/biweekly20230528/serialporttool.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

