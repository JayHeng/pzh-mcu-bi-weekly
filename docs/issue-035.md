# 痞子衡嵌入式半月刊： 第 35 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 34 期》](https://www.cnblogs.com/henjay724/p/14935868.html)

## 唠两句

这周三是小暑，历史上的今天：1405年7月11日，明朝航海家郑和开始了他的第一次下西洋的航行。

本期共收录 1条资讯、5个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、华米科技自研 OS 即将发布</font>

7月9日华米科技官方微博发了新一张关于13日Next Beat大会的海报，其中提到“在魔改的捷径面前，并非巨头的我们，凭什么敢走自研OS这条「弯路」。更懂用户、更适合手表的可穿戴系统，4天见”，宣布发布自研可穿戴操作系统的消息。

除了自研OS，华米还将发布新一代的黄山芯片，除了独立GPU，还首次采用了双核RISC-V架构，算力更强，功耗更低，让我们拭目以待。

![](http://henjay724.com/image/biweekly20210711/huami_7_13_next_beat.jpg)

## 项目类

### <font color="red">1、TBOX - 一个用 C 语言实现的跨平台开发库</font>

TBOX 是一个用c语言实现的跨平台开发库。针对各个平台，封装了统一的接口，简化了各类开发过程中常用操作，使你在开发过程中，更加关注实际应用的开发，而不是把时间浪费在琐碎的接口兼容性上面，并且充分利用了各个平台独有的一些特性进行优化。这个项目的目的，是为了使C开发更加的简单高效。

> 项目主页： https://github.com/tboox/tbox/

TBOX 目前支持的平台有: Windows, Macosx, Linux, Android, iOS, *BSD等等。

![](http://henjay724.com/image/biweekly20210711/tbox-xscode.png)

### <font color="red">2、ART-Pi - RT-Thread 推出的 DIY 开源硬件</font>

ART-Pi 是 RT-Thread 团队经过半年的精心准备，专门为嵌入式软件工程师、开源创客设计的一款极具扩展功能的 DIY 开源硬件。

ART-Pi 硬件具备性能强大的主控 STM32H750，实用的外设，丰富的扩展接口，是 RT-Thread 团队耗时半年精心打磨出来的精品，也是学习、DIY、产品原型验证的不二之选。

> 项目官网： https://art-pi.gitee.io/website/
> 项目主页： https://github.com/RT-Thread-Studio/sdk-bsp-stm32h750-realthread-artpi

![](http://henjay724.com/image/biweekly20210711/ART-Pi_HW_board.PNG)

![](http://henjay724.com/image/biweekly20210711/ART-Pi_BlockDiagram.PNG)

### <font color="red">3、iRTU - 开源 DTU/RTU 解决方案</font>

iRTU 是基于合宙 air202/208/800/801/720/724/H/D/G/U 系列模块的开源DTU/RTU解决方案，已成功运行在上百万设备，安全可靠。

> 项目主页： https://gitee.com/hotdll/iRTU

iRTU 主要功能包括：

```text
1. 支持TCP/UDP socket,支持HTTP,MQTT,等常见透传和非透传模式
2. 支持OneNET,阿里云，百度云，腾讯云等常见公有云。
3. 支持RTU主控模式
4. 支持数据流模版
5. 支持消息推送(电话，短信，网络通知)
6. 支持GPS数据以及相关数据采集
7. 支持ADC,I2C等外设，可以方便的扩展为屏幕、二维码等解决方案.
8. 需要将配置文件烧录到固件的，修改源码irtu.cfg文件，然后打包源码+lib+core 成固件即可; irtu.cfg 内包含demo，可以用web导出的配置json文件替换''(单引号内的json字符串)即可。
```

### <font color="red">4、mbedTLS - 最小巧的 SSL 加密库</font>

mbedTLS 原名 PolarSSL，是一个开源、可移植、易于使用、代码可读性高的SSL库。PolarSSL 于 2014 年被 ARM 公司收购，并改名为 mbedTLS。

> 项目主页： https://github.com/ARMmbed/mbedtls

mbedTLS 可实现常用的加密/解密算法，X.509 证书操作以及 TLS/DTLS 协议。它的各个功能模块相对独立、耦合低，可以通过配置宏定义裁剪，非常适合用于嵌入式系统。mbedTLS 目前由 TrustedFirmware 维护。

### <font color="red">5、LwIP - 小型开源 TCP/IP 协议栈</font>

LwIP 是瑞典计算机科学院(SICS)的 Adam Dunkels 开发的一个小型开源的 TCP/IP 协议栈。 LwIP 的设计初衷是：用少量的资源消耗(RAM)实现一个较为完整的 TCP/IP 协议栈。

> 项目官网： http://savannah.nongnu.org/projects/lwip/

LwIP 有无操作系统的支持都可以运行，它只需十几 KB 的 RAM 和 40KB 左右的 ROM 就可以运行，这使得 LwIP 协议栈适合在低端的嵌入式系统中使用。

LwIP 具有主要特性如下：

```text
1. 支持 ARP 协议（以太网地址解析协议）。
2. 支持 ICMP 协议（控制报文协议），用于网络的调试与维护。
3. 支持 IGMP 协议（互联网组管理协议），可以实现多播数据的接收。
4. 支持 UDP 协议(用户数据报协议)。
5. 支持 TCP 协议(传输控制协议)，包括阻塞控制、 RTT 估算、快速恢复和快速转发。
6. 支持 PPP 协议（点对点通信协议） ，支持 PPPoE。
7. 支持 DNS（域名解析）。
8. 支持 DHCP 协议，动态分配 IP 地址。
9. 支持 IP 协议，包括 IPv4、 IPv6 协议，支持 IP 分片与重装功能，多网络接口下的数据包转发。
10. 支持 SNMP 协议（简单网络管理协议）。
11. 支持 AUTOIP，自动 IP 地址配置。
12. 提供专门的内部回调接口(Raw API)，用于提高应用程序性能。
13. 提供可选择的 Socket API、 NETCONN API (在多线程情况下使用) 。
```

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

