# 痞子衡嵌入式半月刊： 第 105 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 104 期》](https://www.cnblogs.com/henjay724/p/18302000)

## 唠两句

历史上的今天：

本期共 4 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、DC-UPS - 开源小型直流60W UPS电源</font>

DC-UPS 是一种小型直流 UPS 电源，设计用于在停电时保持小型电器如小型交换机、家庭路由和 WLAN 接入点等网络设备运行。

 * 项目地址：https://github.com/TobleMiner/DC-UPS

DC-UPS 特性包括：

```text
- 包含3个直流输出
- 输出电压可选(9V/12V/12.5V/15V)
- USB-C电源输出(仅5V, 3A)
- 内置，易于更换电池(2个锂电池18650)
- 开源固件(基于esp32, esp-idf框架)
- 简单的软件更新，通过USB端口
```

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-105/DC-UPS.PNG)

 ### <font color="red">2、Moddable SDK - 为嵌入式软件开发带来JavaScript生态系统</font>

Moddable SDK 改变了嵌入式软件的构建方式，它将为网络提供动力的 JavaScript 语言引入为消费者和工业物联网产品提供动力的低成本硬件。软件开发人员现在可以自由地使用许多标准的 web 开发工具，而不必纠结于专有的嵌入式 sdk。modable SDK 集成了对网络、传感器、视觉丰富的触摸显示、安全、音频、数据存储等的支持。

 * 项目地址：https://github.com/Moddable-OpenSource/moddable

基于 Moddable SDK 开发的产品界面效果：

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-105/ModdableSDK.PNG)

 ### <font color="red">3、Joulescope - 廉价、精密的功耗分析仪</font>

Joulescope 是一款经济实惠的精密能量分析仪，它能精确地同时测量提供给目标设备的电压和电流，然后计算功率和能量。最早是在 kickstarter 上发起的众筹项目，发布时开源了图形用户界面(UI)，UI 在主机上运行，并通过 USB 与 Jouescope 设备通信。

 * 项目地址：https://github.com/jetperch/pyjoulescope_ui

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-105/Joulescope-1.PNG)

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-105/Joulescope-2.PNG)

 ### <font color="red">4、OMOTE - 基于ESP32和LVGL的开源万能遥控</font>

OMOTE 是一个基于 ESP32 的开源通用遥控器。它的电容式 2.8 英寸触摸屏为切换设备和设置提供了直观而快捷的用户界面。由于遥控器具有红外、Wi-Fi和蓝牙连接功能，因此不需要集线器或坞站。由于其优化的功耗，OMOTE 充电一次可以运行数月。其所有设计文件都是开源的，可以根据自己的设备和需求完全定制它们。

 * 项目地址：https://github.com/CoretechR/OMOTE

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-105/OMOTE.gif)

## 工具类

### <font color="red">1、fq - 支持各种流媒体格式解析的小软件</font>

fq 受 jq 工具和语言的启发，允许用户以相同的方式处理二进制格式。除了使用 jq 表达式，它还可以显示解码的树结构，转换，切片和连接二进制数据。它还支持嵌套格式，并具有可自动完成函数和名称的交互式 REPL。fq 最初设计用于查询、检查和调试媒体编解码器和容器，如 MP4、FLAC和JPEG，但后来扩展到支持各种格式。

 * 工具地址：https://github.com/wader/fq

fq 支持的格式如下：  

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-105/fq-formats.PNG)

fq 解析效果如下：  

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-105/fq.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

