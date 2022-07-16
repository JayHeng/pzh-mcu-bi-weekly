# 痞子衡嵌入式半月刊： 第 58 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 57 期》](https://www.cnblogs.com/henjay724/p/16412147.html)

## 唠两句

历史上的今天：1968年7月16日，世界最大的半导体公司，英特尔公司成立。

本期共收录 2个项目、3个工具，希望对你有帮助！

## 项目类

### <font color="red">1、CANT - CAN总线模拟实现</font>

I/O 方式模拟 UART, SPI, I2C 协议的有很多，但是模拟 CAN 协议的却很少，今天介绍的 CANT 就是 CAN 总线模拟实现，原项目是在 ST Micro Nucleo-H743ZI 板子上示例的。作者近期推出了一个C和Python包 - canhack，方便大家移植到各种不带 CAN 的芯片。

> * 项目地址1：https://github.com/bitbane/CANT
> * 项目地址2：https://github.com/kentindell/canhack

![](http://henjay724.com/image/biweekly20220716/CANT.PNG)

### <font color="red">2、SimplePnP - 开源的PCB贴装机</font>

印刷电路板组装是制造电子器件的关键环节。大批量的PCB通常由工厂流水线上的专门机器处理，而原型通常是手工制作的。手工组装是缓慢、困难和极其乏味的，SimplePnP 被设计成可靠、准确、价格合理，并适用于各种各样的组件。对于电子创业公司、发明家、研究人员和黑客空间来说，它是一个很好的选择。

> * 项目主页：https://www.crowdsupply.com/citrus-cnc/simplepnp

![](http://henjay724.com/image/biweekly20220716/SimplePnP.PNG)

SimplePnP 与其它两款平台的比较：

![](http://henjay724.com/image/biweekly20220716/SimplePnP_VS.PNG)

## 工具类

### <font color="red">1、Wireshark - 最广泛使用的开源网络协议分析器</font>

Wireshark 是世界上最重要的、被广泛使用的网络协议分析器。Wireshark 可以从以太网，IEEE 802.11, PPP/HDLC, ATM，蓝牙，USB，令牌环，帧中继，FDDI和其他(取决于你的平台)读取实时数据。

> * 软件官网：https://www.wireshark.org/

Wireshark 包含许多协议的解密支持，包括IPsec、ISAKMP、Kerberos、SNMPv3、SSL/TLS、WEP和WPA/WPA2。下面是 Wireshark 联合 USBpcap 驱动做得 USB 抓包示例。

![](http://henjay724.com/image/biweekly20220716/Wireshark.PNG)

### <font color="red">2、SD Card Formatter - SD卡联盟发布的SD/SDHC/SDXC格式化小软件</font>

SD卡联盟强烈强烈建议使用此软件来格式化 SD/SDHC/SDXC 卡，而不要使用各个操作系统随附的格式化工具。通常，操作系统附带的格式化工具可以格式化包括 SD/SDHC/SDXC 卡在内的各种存储介质，但是可能无法针对 SD/SDHC/SDXC 卡进行优化，并且可能导致性能降低。

FatFS 作者 ChaN 老师也建议大家不要使用操作系统自带的工具来格式化。

> * 软件下载：https://www.sdcard.org/downloads/formatter/

![](http://henjay724.com/image/biweekly20220716/SD_Card_Formatter.PNG)

### <font color="red">3、Altium 365 Viewer - Altium出品的在线PCB查看器</font>

Altium 出品的线上PCB Viewer，对于没有安装PCB软件的用户来说，查看PCB将非常方便。本地 PCB 文件上传上去之后还可以很方便地分享给其他人。这个软件同时也支持 KiCad 格式。

> * 软件官网：https://www.altium.com/viewer/

![](http://henjay724.com/image/biweekly20220716/Altium-365-Viewer.gif)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

