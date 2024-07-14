# 痞子衡嵌入式半月刊： 第 104 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 103 期》](https://www.cnblogs.com/henjay724/p/18279067)

## 唠两句

历史上的今天：

本期共 4 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、M17 - 开源业余无线电套件</font>

M17 是一个由开源开发者和无线电爱好者组成的社区，社区正在开发开源硬件、软件，并为业余无线电操作员提供完整的数据和语音数字无线电协议。协议的语音模式使用免费和开放的 Codec 2 语音编码器。

 * 项目地址：https://github.com/M17-Project

硬件部分包含一个完整的低射频功率 I/Q 收发器，能够支持几乎任何模式(包括M17和FreeDV)。它是围绕 AT86RF215 芯片构建的，由 Microchip/Atmel 和 Lattice 的 LIFCL-40-9SG72C FPGA 作为 stm32f469 板的屏蔽。该板可以与其他 MCU 平台配合使用。

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-104/M17.png)

### <font color="red">2、DeviceScript - 用于微型物联网设备的编程语言</font>

DeviceScript 为基于低资源微控制器的设备带来了 TypeScript 开发人员的体验，DeviceScript 被编译成一个定制的 VM 字节码，它可以在非常受限的环境中运行。

 * 项目地址：https://github.com/microsoft/devicescript/

DeviceScript 特点包括：

```text
- 类似 TypeScript 熟悉的语法和工具
- 小内存占用 DeviceScript 字节码解释器
- 在抽象硬件服务之上编写可重用的应用程序/固件
- 专为低功耗，低闪存，低内存嵌入式项目
- 使用模拟或真实的传感器开发和测试固件
- 完整的调试经验，在Visual Studio Code，硬件或模拟设备
- 利用npm、yarn或pnpm来分发和使用DeviceScript包。
```

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-104/DeviceScript.png)

### <font color="red">3、usb-switch - 软硬件全开源的USB-C双向切换器</font>

usb-switch 是 USB-C 双向切换器，它可以实际控制 USB 设备和主机之间的切换连接，对于 USB-C 的基础功能都支持，如高速通信和充电功能。这个项目主要解决了一个主机和多个设备，或者一个设备和多个主机的无痛切换问题。

 * 项目地址：https://gitlab.com/CodethinkLabs/usb-switch

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-104/usb-switch.PNG)

### <font color="red">4、rogowski-relief - 基于罗氏线圈的电流探头</font>

该项目是一个基于 rogowski 线圈的电流探头，旨在测量狭小空间中的高频交流电流。感应线圈被优化得足够小，可以安装在 to -220 晶体管的引线之间，并且可以绕着许多通孔功率元件的引线滑动，以进行非侵入式电流测量。该项目由 rogowski 线圈和积分器/放大器组成，积分器/放大器调节来自 rogowski 线圈的信号，并提供与流过由 rogowski 线圈环绕的导体的电流成比例的输出电压。

 * 项目地址：https://github.com/westonb/rogowski-relief

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-104/rogowski-relief.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

