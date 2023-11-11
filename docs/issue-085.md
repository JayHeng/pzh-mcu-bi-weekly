# 痞子衡嵌入式半月刊： 第 85 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 84 期》](https://www.cnblogs.com/henjay724/p/17810326.html)

## 唠两句

历史上的今天：。

本期共收录 3 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、NetX Duo - 专为深度嵌入式实时应用设计的TCP/IP网络堆栈</font>

Azure RTOS NetX Duo 嵌入式 TCP/IP 网络堆栈是 Microsoft 高级行业级 IPv4 和 IPv6 TCP/IP 双网络堆栈，专为深度嵌入式实时应用程序和 IoT 应用程序而设计。 NetX Duo 为嵌入式应用程序提供 IPv4、IPv6、TCP 和 UDP 等核心网络协议以及一整套其他更高级别的附加协议。 

 * 项目地址：https://github.com/azure-rtos/netxduo

NetX Duo 包含了适用于 Azure RTOS 的 Azure IoT 中间件，这是一个特定于平台的库，充当 Azure RTOS 和 Azure SDK for Embedded C 之间的绑定层，从而与 Azure IoT 服务建立连接。 

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-085/NetX_Duo.PNG)

### <font color="red">2、Zorb-Framework - 基于面向对象思想的轻量级嵌入式框架</font>

Zorb Framework 是一个轻量级的嵌入式框架，搭建目的是为在不能运行 Linux 的芯片上快速开发应用，不用反复造轮子。

> * 项目地址：https://github.com/54zorb/Zorb-Framework

Zorb Framework 的初步设计功能有：

```text
​1、时间系统功能zf_time
​2、环形缓冲区功能zf_buffer
​3、列表功能zf_list
​4、状态机功能zf_fsm
​5、事件功能zf_event
​6、定时器功能zf_timer
​7、任务功能zf_task
```

前6个功能可以实现纯事件驱动的程序，基本可以满足中小型嵌入式应用程序开发的需求。加上任务功能，即可满足部分程序对实时性要求较高的需求。

### <font color="red">3、try.c - C语言实现的try catch异常捕获</font>

try catch 的作用是当程序发生错误时，能够保证程序继续执行下去，在 Java/C++/Python 上有专门的 try catch 供调用。本项目基于 C 语言做了实现。 

 * 项目地址：https://github.com/madler/pigz/blob/master/try.c

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

