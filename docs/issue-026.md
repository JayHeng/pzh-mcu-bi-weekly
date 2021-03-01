# 痞子衡嵌入式半月刊： 第 26 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 25 期》](https://www.cnblogs.com/henjay724/p/14399544.html)

## 唠两句

雨水是上周四的事了，本期又延后了11天，干脆以后都在节气后十天给大家带来半月刊吧。二十四节气小知识在鼠年给大家都介绍过一遍了，牛年咱们换为历史上的今天：772年2月28日，白居易出生，与元稹创建“元白”诗派，后人称之为“诗魔”。

本期共收录 2条资讯、4个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、KIOXIA铠侠和西部数据联合宣布推出第六代3D闪存技术</font>

今天铠侠和西部数据两家公司联合宣布，它们已经开发了第六代162层3D闪存技术。KIOXIA和西部数据在全球总计生产了30％以上的闪存，第六代闪存技术是两家公司迄今为止利用创新技术实现的最高密度和最先进的3D闪存技术。

> 资讯主页: https://business.kioxia.com/en-jp/news/2021/20210219-1.html

![](http://henjay724.com/image/biweekly20210221/KIOXIA.PNG)

随着摩尔定律在整个半导体行业达到其物理极限，但在某些技术领域地方，摩尔定律仍在不断发展着相关性。为了继续进步并满足全球不断增长的数据需求，一种新的3D闪存缩放方法的研究是至关重要的。对于这新一代产品，铠侠和西部数据在垂直和横向缩放方面引入了创新技术，从而在具有更少层数的更小的裸片中实现更大的容量。

第六代3D闪存具有超越传统八交错存储孔阵列的先进体系结构，与第五代技术相比，横向单元阵列密度提高了10％。与112层堆叠技术相比，这种横向缩放的进步与162层堆叠的垂直存储器相结合，使芯片尺寸减小了40％，与上一代产品相比，它们的程序性能提高了近2.4倍，读取延迟提高了10％， I/O性能也提高了66％，从而使下一代接口能够满足对更快的传输速率不断增长的需求。

### <font color="red">2、恩智浦等五家行业领导厂商联合打造汽车数据生命周期平台Fusion Project</font>

恩智浦半导体、Airbiquity、Cloudera、Terak和Wind River近日宣布开展Fusion Project项目，这是一个专为汽车制造商打造的端到端的数据生命周期平台，以推动智能互联车辆的发展。计划通过预先集成的软硬件解决方案，并结合当前最领先的创新技术，使互联车辆的数据能够被汽车制造商高效地收集、分析并做进一步管理，从而达到连续的功能开发、部署和演进的目的。

> 资讯主页: https://www.nxp.com.cn/company/about-nxp/newsroom/the-fusion-project:THE-FUSION-PROJECT

![](http://henjay724.com/image/biweekly20210221/NXP.PNG)

据悉，Fusion Project项目的第一个应用是利用各企业的协同技术指定智能车辆车道变更检测解决方案。该解决方案合各家之所长被打造，创建了一个功能强大、高效的数据生命周期平台，涵盖从数据获取到OTA机器学习模型更新的各个环节，在不损害数据保真度的同时，最大限度地提高了系统决策的准确性。

```text
- Airbiquity – 无线(OTA)软件管理
- Cloudera – 从边缘到AI的数据生命周期解决方案
- 恩智浦 – 汽车处理平台
- Teraki – 边缘数据人工智能(AI)
- Wind River – 智能系统平台软件
```

## 项目类

### <font color="red">1、Watchy - 带有开源硬件和软件的电子墨水手表</font>

Watchy是带有开源硬件和软件的电子墨水手表。它采用准系统设计，利用PCB作为表体，可以按原样佩戴，也可以使用不同的3D打印表壳和表带进一步定制。它既是独特的时计，又是可穿戴的开发平台，可让用户创造自己的体验。

> * 官方网站: https://watchy.sqfmi.com/
> * 项目主页: https://github.com/sqfmi/Watchy

Watchy的E-Ink显示屏可在明亮的阳光下清晰可见地始终显示美丽，清晰的图像，并且在两次更新之间不需要电源。显示屏为200 x 200像素和单色，具有独特的美感。Watchy同时具有Wi-Fi和Bluetooth LE连接功能，可以与Internet API（例如天气，新闻，交通，地图，Spotify等）以及支持Bluetooth LE的设备连接。

![](http://henjay724.com/image/biweekly20210221/Watchy.PNG)
-
![](http://henjay724.com/image/biweekly20210221/Watchy_blocks.PNG)

### <font color="red">2、stm32_weather - 支持语音识别的智能桌面天气预报系统</font>

这是一个简易的智能桌面天气预报系统，整个系统基于STM32单片机，ESP8266WIFI模块，TEA5767收音机模块，LD3320语音识别模块，SYN6288语音合成模块以及各类环境传感器模块搭建而成，一个简单的液晶显示界面支持天气预报的显示，中英文键盘输入，收音机调频等功能。

> 项目主页: https://github.com/zhengnianli/stm32_weather

![](http://henjay724.com/image/biweekly20210221/stm32_weather.JPG)

通过简单的对话和以及关键词的识别，能够实现初步的人机交互。智能桌面天气预报系统支持的具体功能如下：

```text
1. 实时天气显示,温湿度显示,日历显示;
2. 空气质量显示;
3. 收音机功能;
4. 语音识别功能，可用语音搜索天气；
5. 可用触摸屏搜索天气。
```

### <font color="red">3、CASIO F-91W - 挂墙上的电子手表</font>

CASIO F-91W 是由日本卡西欧电子公司生产的一款非常经典的石英数字式手表，自1989 年推出以来，凭借其可靠和简洁的设计而广受欢迎，曾一度被美军视为“基地组织的标志”。如何把下面这款电子手表制作并挂在家里的墙上，下面带来详细的教程：

> 项目主页: https://make.quwj.com/project/294

![](http://henjay724.com/image/biweekly20210221/Watch.png)

整个系统的硬件原理图架构如下图所示，配备Nextion HMI 7''显示器，Nextion  IO适配器，Arduino数字时钟模块，USB转TTL转型转换模块，蜂鸣器，LED灯，TTP223触摸传感器灯...使用 USB 连接到 TTL 串行转换器，将代码从 Nextion 编辑器下载到 HMI 显示器。使用 5V 移动电源或 DC 5V 1A 适配器为 Arduino 供电，具体的Arduino 代码文件，可以从在项目链接地址下载。最后将3D打印好的表壳，纽扣，搭扣，以及2D打印的表带等零部件组装在一起，成本就完成了。

![](http://henjay724.com/image/biweekly20210221/Watch2.JPG)

### <font color="red">4、MicroByte - 一款DIY复古游戏机</font>

MicroByte 是一款微型复古游戏机，能够支持运行的游戏系统高达5种，并且元器件都设计在这 78 x 17 x 40 mm 的封装中，尺寸很小，诚聘精致，符合SNES 游戏板的布局并且具有操作按钮。

> 项目主页: https://make.quwj.com/project/359

```text
-NES
-GameBoy
-GameBoy Color
-Game Gear
-Sega Master 
```

![](http://henjay724.com/image/biweekly20210221/MicroByte.png)

MicroByte的显示屏采用的是 IPS 1.3 英寸的屏幕，分辨率为 240 x 240，可以提供非常漂亮的色彩和清晰的图像。通信协议是为SPI，可以实现高达 70 FPS 的帧速率。另一方面，可以控制显示器的背光以选择亮度等级，通过 BS138 MOSFET 晶体管完成控制显示屏上嵌入的 LED 的电流。采用 MAX98357作为 音频放大器。驱动接扬声器或耳机，提供 6.4W 的输出功率。整个项目 的固件、原理图设计、PCB 设计、外壳 3D 文件，BOM 清单等都能从本项目的文件库中下载得到。

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

