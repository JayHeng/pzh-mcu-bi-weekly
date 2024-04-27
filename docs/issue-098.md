# 痞子衡嵌入式半月刊： 第 98 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 97 期》](https://www.cnblogs.com/henjay724/p/18125131)

## 唠两句

历史上的今天：。

本期共收录 3 个项目、0 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、P-Net - 一个用C语言编写的Profinet IO设备</font>

P-Net 是一个 Profinet IO 设备，用C语言编写，可以在裸机硬件、RTOS(如RT-Kernel)或 Linux 上运行。主要要求是平台可以发送和接收 RAW 以太网第2层帧。Profinet 堆栈提供了完整的源代码，包括一个移植层。P-Net 易于使用，占用空间小，特别适合于资源有限且效率至关重要的嵌入式系统。

 * 项目地址：https://github.com/rtlabs-com/p-net

 ### <font color="red">2、onps - 一个开源且完全自主开发的国产网络协议栈</font>

onps是一个开源且完全自主开发的国产网络协议栈。设计目标与 LwIp 相同，onps 栈的目标系统同样是资源受限的单片机系统。提供完整的 tcp/ip 协议族实现，同时提供 sntp、dns、ping 等网络工具，支持以太网环境下 dhcp 动态 ip 地址申请，也支持动态及静态路由表。协议栈还封装实现了一个伯克利套接字（Berkeley sockets）层。协议栈使用ANSI C语言开发。

 * 项目地址：https://gitee.com/Neo-T/open-npstack

onps 栈设计实现了一套完整的 tcp/ip 协议模型。从数据链路层到ip层，再到tcp/udp层以及之上的伯克利socket层，最后是用户自己的通讯应用层，onps栈实现了全栈覆盖，能够满足绝大部分的网络编程需求。其架构如下：

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-098/onps.jpg)

 ### <font color="red">3、lcd-clock - 一个非常低功耗的LCD时钟</font>

这是一个非常低功耗的 LCD 时钟，基于 AVR128DA48，使用 CR2032 纽扣电池能够运行超过三年。每分钟它会简短地显示温度，使用 AVR128DA48 的片上温度传感器，和电池电压，通过使用 ADC 读取自己的电源电压。还有一个 I2C 连接，所以你可以添加一个外部传感器，例如，除了显示其他读数外，还可以显示湿度。

 * 项目地址：https://github.com/technoblogy/lcd-clock

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-098/lcd-clock.PNG)

## 工具类



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

