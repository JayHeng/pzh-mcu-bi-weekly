# 痞子衡嵌入式半月刊： 第 11 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 10 期》](https://www.cnblogs.com/henjay724/p/13174275.html)

## 唠两句




本期共收录 3条资讯、2个项目、2个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、兆易创新与IAR联合发布RISC-V解决方案</font>

日前，IAR Systems宣布与兆易创新达成合作伙伴关系，将为兆易创新基于RISC-V内核的MCU产品提供性能强大的开发工具。同时，双方合作将为RISC-V开发者提供易于使用的完整解决方案。

> 资讯主页: https://www.iar.com/iar-embedded-workbench/tools-for-risc-v/evaluation-kit-for-risc-v/

![](http://henjay724.com/image/biweekly/IAR_GD32V.jpeg)

兆易创新作为业界领先的Flash和MCU供应商，致力于提供先进的存储技术和IC解决方案。2019年8月，兆易创新推出了全球首个基于RISC-V内核的32位通用微控制器，而随着RISC-V技术和生态系统的迅速发展，对于专业开发工具的需求也在增加。

IAR Systems与兆易创新达成的密切合作将把IAR Systems领先的编译器和调试器技术带给兆易创新的RISC-V MCU用户，从而在降低功耗和丰富的外围设备之间发挥均衡的处理能力。这项合作将使成千上万的公司基于RISC-V技术创建功能强大、易于使用的完整解决方案。

### <font color="red">2、华米“黄山2号”可穿戴芯片发布：AI性能提升7倍，功耗降低50%！</font>

华米科技近日正式发布了新一代智能可穿戴芯片“黄山2号”，预计将于今年四季度量产。明年（2021年）上半年，搭载“黄山2号”的可穿戴新品也将面世。

> 资讯主页: https://www.huami.com/news/118

![](http://henjay724.com/image/biweekly/Huami_MHS002.jpg)

和“黄山1号”一样，“黄山2号”仍基于先进的RISC-V架构，RISC-V被公认为是IoT（物联网）时代最具潜力的芯片架构。它具有高运算效率和低使用功耗两大优势，相比于在可穿戴设备中常用的ARM Cortex-M4架构处理器，整体运算效率提升了38%｡

华米科技为“黄山2号”重新设计了AI本地生物数据计算NPU，采用卷积神经网络加速技术，大大提升了本地AI数据计算的性能，加快了识别速度。基于心率数据，“黄山2号”的房颤识别速度是“黄山1号”的7倍，是市面上其它软件算法的 26 倍。

同时，“黄山2号”还加入了超低功耗传感器AON模式，和苹果一样搭载了协处理器-C2协处理器。该处理器可单独用于数据收集，能在主芯片处于休眠甚至关闭状态时，仍持续保持健康数据的记录工作；理论上可使黄山2号整体功耗下降50%，从而让用户彻底告别可穿戴设备的续航焦虑。

### <font color="red">3、米唐科技推出了模组、算法、软件一体的VUI Turnkey解决方案Sugr Sense A</font>

基于英飞凌 XENSIV™ MEMS高性能麦克风 IM69D130，Sugr米唐科技推出了模组、算法、软件一体的VUI Turnkey解决方案——Sugr Sense A，并且一次测试就通过了亚马逊AVS认证。

> 方案主页: https://www.sugrsense.com/products/1

Sugr Sense A特性如下：

```text
Voice Service： Amazon Alexa & Tencent XiaoWei
CPU：           Amlogic A113x Quad-ARM Cortex-A53 1.5GHz
System：        Linux 4.9
DMIC：          4x DMIC
Wi-Fi：         WiFi 802.11 a/b/g/n/ac (2.4GHz and 5.8GHz)
Bluetooth：     BT4.2 BLE+BT2.1EDR
Algorithm：     SSP, BF, NR, RR, AEC, NLP, Far field pickup
```

Sugr Sense A可集成在各式各样的智能设备上，例如这次就集成在筒灯设备，将语音交互功能部署在室内的各个角落，并联动控制各类智能产品（如开关灯指令），实现更自然的语音交互体验，自此“君子动口不动手”在智能时代被赋予了全新的含义~

![](http://henjay724.com/image/biweekly/Sugr-Sense-A.png)

远场拾音？即时响应？多语言支持？联网设备控制？作为一款领先的智能语音交互方案，这些特性当然统统都有。Sugr Sense A支持Alexa Call & Message（ACM）与Multi-room Music（MRM）等关键的Alexa语音助手功能，AVS认证资质专为国际市场打造，并支持英语、法语、西班牙语、德语、意大利语等多门通用语言。当然，除了Alexa，Sugr Sense A也支持其他的智能语音交互平台，更可以集成到其他的智慧家居、智慧生活产品中。

## 项目类

### <font color="red">1、NES-Game - 基于 ESP32 的自制掌上游戏机</font>

自制游戏机项目每年都会推陈出新，今天要为大家介绍的是基于 ESP32 和 ATtiny861 来构建任天堂 NES 游戏模拟器掌机。

> 项目主页: https://make.quwj.com/project/117
> 项目源码: https://github.com/moononournation/esp32-nesemu

该项目给出了所有材料清单，并且有超级详细的教程教你从硬件制作到软件下载一步一步地完成这个设计。对于电子工程师来说，动手能力是很重要的技能，这也是电子工程师区别于程序员的重要特质。

![](http://henjay724.com/image/biweekly/ESP32_ATtiny861_gameboy.jpg)

### <font color="red">2、RPI_web_remote_control - 基于树莓派和web界面的远程家电控制器</font>

RPI_web_remote_control是一个利用网页远程控制树莓派发出红外信号控制空调等家电的项目，简单来说，可以在回家的路上用手机通过网页控制，提前将空调打开，设定成需要的温度。同时可以在网页上实时监控室内的温度和湿度。整个项目基于Python的flask框架编写。

> 项目主页:https://github.com/zyzisyz/RPI_web_remote_control

RPI_web_remote_control所用到的元器件如下：

```text
1. 树莓派3B+ ×1
2. SD卡（8GB） ×1
3. 红外发射和接收模块 ×1
4. 温湿度传感模块 ×1
5. 发光二极管 x1
6. 树莓派拓展板 x2
7. 杜邦线 若干
8. 具有公网IP的VPS x1
```

## 工具类

### <font color="red">1、MQTT.fx - 一款超级好用的 MQTT 客户端</font>

MQTT.fx 是一款基于 Eclipse Paho，使用 Java 语言编写的 MQTT 客户端工具，支持通过 Topic 订阅和发布消息，用来前期和物联网云平台调试非常方便。

> 软件主页: http://mqttfx.jensd.de/

![](http://henjay724.com/image/biweekly/MQTT-fx.PNG)

在云端创建产品后，一般都不会直接使用SDK对接，而是先测试一下对接接口是否可以正常使用！该工具目前测试可以对接百度云、华为云，以及自己使用EMQ-X搭建的Mqtt服务器，非常方便。

### <font color="red">2、excel2json - 能够将Excel数据转换成Json格式的工具</font>

在游戏项目中一般都需要由策划制作大量的游戏内容，其中很大一部分是使用Excel表来制作的，于是程序就需要把Excel文件转换成程序方便读取的格式例如json。excel2json工具正是由此而来，能够将excel数据转换成json数据，效率非常高。

> 项目主页: https://github.com/neil3d/excel2json

excel2json主要支持以下三个功能：

```text
1. 支持读取 Excel 97-2003的 .xls格式和2007的 .xlsx格式；
2. 支持多个表单导出；
3. 把Excel表单转换成Json对象，并保存到一个文本文件中。支持将表中内容转换成Array，或者以第一列为ID的字典对象；
```

![](http://henjay724.com/image/biweekly/Exceljson.PNG)
