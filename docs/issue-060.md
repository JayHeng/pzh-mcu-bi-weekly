# 痞子衡嵌入式半月刊： 第 60 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 59 期》](https://www.cnblogs.com/henjay724/p/16535273.html)

## 唠两句

历史上的今天：1999年8月9日，中国科技部开始设立国家最高科学技术奖。这一奖项个人奖金为500万元人民币，其中50万元属获奖者个人所得，450万元由获奖者自主选题，用作科学研究经费。

本期共收录 1 个项目、5 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、Cyclone TCP - 专用于嵌入式应用的双IPv4/IPv6栈</font>

CycloneTCP 是专用于嵌入式应用的双 IPv4/IPv6 栈。CycloneTCP 符合 RFC 标准，并提供与现有的 TCP/IP 系统的无缝互操作性。通过支持 IPv6，CycloneTCP 简化了下一代互联网的部署。该协议栈作为完整的 ANSI C 和高度可维护的源代码发布。

> * 项目地址：https://www.oryx-embedded.com/products/CycloneTCP

CycloneTCP 主要特性: 

```text
- 双协议栈（IPv4和/或IPv6）
- 内置对多个网络接口的支持
- 灵活的内存占用（构建时配置，只嵌入必要的功能）
- 可配置存储器模型（静态内存池或堆内存配置）
- 便携式架构（无处理器依赖关系）
- 适用任何RTOS的简单直接端口
- 高度可维护的源代码
- 可简化开发与集成的调试与跟踪功能
- BSD型套接字API
- 阻塞/非阻塞套接字操作与事件驱动函数（选择和轮询）
- 通过零复制实现高效数据传输
- 精心设计的TCP模块，支持选择性确认(SACK)与拥塞控制
- 原始套接字接口
- IP分片与重组支持
- 支持虚拟接口（每个物理接口有多个MAC地址）
- 支持多宿主主机（每个接口有多个IPv4地址）
- 使用VLAN标记或尾部标记扩容以太网端口
- VLAN支持（802.1q和802.1ad）
- USB设备RNDIS类驱动（适用于STM32微控制器）
- STM32评估板（Nucleo、Discovery、Eval）提供演示项目
```

![](http://henjay724.com/image/biweekly20220807/CycloneTCP.PNG)

## 工具类

### <font color="red">1、EWPtool - 从其他工具链迁移到IAR的项目迁移工具</font>

EWPtool 是 IAR 官方出品的项目迁移工具，能够将几乎任何项目迁移到 IAR。该工具还允许在工具链的不同版本之间进行迁移。通过使用 EWPtool，迁移变得简单而高效。

> * 工具地址：https://github.com/IARSystems/project-migration-tools

EWPtool 目前支持的工具链包含 Keil μVision、Atollic TrueSTUDIO、Renesas HEW、Renesas CS+、Texas Instruments Code Composer Studio 等。

![](http://henjay724.com/image/biweekly20220807/EWPtool.PNG)

### <font color="red">2、WebRISC-V - 基于web的面向教育的RISC-V仿真环境</font>

WebRISC-V 是一个基于 web 的图形流水线数据路径仿真环境，为 RISC-V 指令集架构构建。它适用于教授汇编级代码是如何在 RISC-V 流水线架构上执行的，并用于演示流水线架构元素。

> * 工具地址：https://webriscv.dii.unisi.it/
> * 工具地址：https://github.com/Mariotti94/WebRISC-V

![](http://henjay724.com/image/biweekly20220807/WebRISC-V.PNG)

### <font color="red">3、USBDeview - USB驱动查看和卸载软件</font>

USBDeview 是一个小的实用程序，列出了当前连接到 PC 的所有 USB 设备，以及以前使用的所有USB设备。USBDeview还允许卸载以前使用的 USB 设备，断开当前连接到 PC 的 USB 设备，以及禁用和启用 USB 设备。

> * 工具地址：http://www.nirsoft.net/utils/usb_devices_view.html

![](http://henjay724.com/image/biweekly20220807/USBDeview.PNG)

### <font color="red">4、Fiddler - 超级强劲的HTTP抓包软件</font>

Fiddler 是位于客户端和服务器端的 HTTP 代理。目前最常用的 http 抓包工具之一，功能非常强大，是 Web 调试的利器。

> * 工具地址：https://www.telerik.com/fiddler

![](http://henjay724.com/image/biweekly20220807/Fiddler.PNG)

### <font color="red">5、I2C-DESIGNER - 德州仪器推出的I2C设计工具</font>

利用 I2C 设计器工具，可快速解决基于 I2C 设计中寻址、电压电平和频率方面的冲突。输入主输入端和从输入端，以自动生成 I2C 树活轻松构建自定义解决方案。此工具可在调试缺失确认、选择上拉电阻器和满足 I2C 总线最大容性负载方面提供指导，从而帮助设计人员节省时间并遵循 I2C 标准。

> * 工具地址：https://www.ti.com.cn/tool/cn/I2C-DESIGNER

![](http://henjay724.com/image/biweekly20220807/I2C-DESIGNER.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

