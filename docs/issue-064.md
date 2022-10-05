# 痞子衡嵌入式半月刊： 第 64 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 63 期》](https://www.cnblogs.com/henjay724/p/16728229.html)

## 唠两句

历史上的今天：

本期共收录 0 个资讯、4 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、VESC - 非常完整的开源无刷电机驱动项目</font>

ESC是 Electric Speed Controller 的缩写，也就是电子调速控制器，简称电调；项目作者是 Benjamin Vedder，所以叫 VESC，就是本杰明电调。这个项目主要分为几个部分，VESC固件，物料清单，VESC硬件，VESC工具软件，是一个非常完整的软硬件项目，并且配套的软件也很出色。  

BLDC 是开源的电机控制器源码，适用于直流电机，直流无刷电机调速，支持方波驱动和FOC驱动，比较关键的是支持无感FOC。

> * 项目主页1：https://github.com/vedderb/bldc

硬件部分是基于STM32F4 芯片，开源了直流无刷电机控制器的硬件原理图，感兴趣的话，可以基于这个项目做一下自己的硬件。

> * 项目主页2：https://github.com/vedderb/bldc-hardware

![](http://henjay724.com/image/biweekly20221005/VSEC-HW.PNG)

项目还配套做了一个基于Qt的直流电机控制器用户界面，用于配置硬件参数，控制和调试控制器。

> * 项目主页3：https://github.com/vedderb/bldc-tool

![](http://henjay724.com/image/biweekly20221005/VSEC-TOOL.PNG)

### <font color="red">2、Mongoose - 开源嵌入式HTTP/Websocket/MQTT库</font>

Mongoose 是一个非常小巧易用的网络库。它为 TCP、UDP、HTTP、WebSocket、MQTT 实现了基于事件驱动的非阻塞 API，非常适合在嵌入式系统上使用。  

> * 项目主页：https://github.com/cesanta/mongoose

Mongoose 解决了广泛的业务需求，如在设备上实现 Web UI 界面、RESTful API 服务、遥测数据交换、产品远程控制、远程软件更新、远程监控等。

### <font color="red">3、dyad.c - 仅1300行代码的C语言异步网络库</font>

dyad.c 是一个基于 C 语言的异步网络库，旨在轻量级、可移植和易用。它既可用于创建小型独立服务器，也可用于为现有的项目提供网络支持。  

> * 项目主页：https://github.com/rxi/dyad

dyad.c 功能纯粹，API 简洁易使用，对于使用者而言，简直就是开箱即用，前提是你需要的一个简单小巧的 TCP Server。另外，其内部的代码实现优雅且巧妙，非常适合初学者用来学习 Linux 网络编程和了解异步处理的本质。

![](http://henjay724.com/image/biweekly20221005/dyad.PNG)

### <font color="red">4、log.c - 简单到傻瓜都会用的日志库</font>

log.c 是一个 C 语言的日志功能模块。其代码简洁，就一个 .c 和 .h 文件，一共 200 行。log.c 设计优雅，打印日志的 API 只有 1 个，并且提供了将 log 输入到不同目标的接口，例如输入到文件，还提供了实现线程安全的接口。  

> * 项目主页：https://github.com/rxi/log.c

## 工具类

### <font color="red">1、WaveDrom - 在线数字时序图渲染引擎</font>

WaveDrom 是一个免费开源的在线数字时序图渲染引擎。它可以使用 JavaScript, HTML5 和 SVG 来将时序图的 WaveJSON 描述转成 SVG 矢量图形，从而进行显示。WaveDrom 可以嵌入到任何网页中。

> * 工具主页：https://wavedrom.com/

![](http://henjay724.com/image/biweekly20221005/WaveDrom.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

