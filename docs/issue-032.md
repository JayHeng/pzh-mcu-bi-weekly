# 痞子衡嵌入式半月刊： 第 32 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 31 期》](https://www.cnblogs.com/henjay724/p/14774980.html)

## 唠两句

上周日(5.23)痞子衡组织了一场苏州做公众号的朋友线下见面会。活动很High，下午组队搞篮球，激烈对抗中距离一下子拉近了；晚上啤酒烧烤小龙虾，玩牌助兴，6个人干掉三箱啤酒。其实痞子衡平时不太喝酒，但是和初次见面的朋友小聚，要想气氛到位，必须推杯换盏，果然人均6瓶酒下去，大家都分享了工作多年来的深刻感悟，这才是聚会的意义。  

下个月中旬痞子衡将会在互推中将这些朋友正式介绍给大家。  

![](http://henjay724.com/image/biweekly20210530/mcu_geek_group2.PNG)

本期共收录 1条资讯、4个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、恩智浦(NXP)全球首个AI应用创新中心于天津正式启动</font>

恩智浦半导体（NXP）近日于天津启动人工智能应用创新中心。创新中心共分两期，一期为人工智能应用示范基地，将集中展示超过100个恩智浦及合作伙伴的前沿技术和终端应用，覆盖智慧城市、智能家居、智能出行、智能工业等多领域。二期项目为人工智能创新实践基地，将通过技术培训和领先的研发平台赋能合作伙伴开展本地化创新，成为与当地生态合作伙伴协作的枢纽，激发创新。

> 咨询主页： https://www.nxp.com.cn/company/about-nxp/worldwide-locations/greater-china/aiot-applications-innovation-center:AIOT-LAB?cid=ps_PRG538900_TAC538909_BAIDU_AIOT_LAB&xid=146

![](http://henjay724.com/image/biweekly20210530/NXP-AIoT_Center.PNG)

## 项目类

### <font color="red">1、Gear-Lib - 适用于IoT/嵌入式/网络服务开发的C基础库</font>

Gear-Lib是一个适用于IOT/嵌入式/网络服务开发的C基础库。软件全部用POSIX C实现，目标是为了跨平台兼容Linux, Windows, Android, iOS。  

> 项目主页：https://github.com/gozfree/gear-lib

目前Gear-Lib中实现了涵盖数据结构、网络库、异步、I/O、多媒体、系统抽象层等方向共34个库。  

![](http://henjay724.com/image/biweekly20210530/Gear-Lib.PNG)

### <font color="red">2、Quantum Platform - 一种轻量级的实时嵌入式框架</font>

QP(Quantum Platform)是一种轻量级的实时嵌入式框架 Real-Time Embedded Framework (RTEF)，提供架构复用和并发编程，可以完成更高概念性完整性的安全代码，并显著提高软件质量。  

> 项目主页：https://www.state-machine.com/products/qp/

QP系列包括QP/C, QP/C++和QP-nano 框架，所有都具有严格的质量控制，详细的记录以及商业许可。QP中用层次状态图（UML活动图）表示的活动对象行为在QP中是有详细说明的。框架支持手工用C或者C++对UML状态机进行编码，也可以由自动代码生成QM模板工具。

![](http://henjay724.com/image/biweekly20210530/Quantum-Platform.PNG)

### <font color="red">3、TraNOR - 2495个晶体管DIY的8位/7MHz的CPU</font>

TraNOR是国外一个叫Dennis Kuschel的哥们做的主频7MHz的8位CPU，还有操作系统并支持I2C和SPI总线，所有设计文件全部开源。

> 项目主页：http://www.mynor.org/tranor

TraNor为100%的分立计算机设计，除了使用现成的ROM、RAM和LCD模块之外，CPU和I/O都是由分立的晶体管组成的 ，4个8位的I/O端口使用了598个晶体管，其它的1897个MOSFETs用来搭建CPU。

作者还开发了一个操作系统，包含了一些有用的API功能，并且还做了支持Linux和Windows的交叉编译器。

![](http://henjay724.com/image/biweekly20210530/TraNOR.PNG)

### <font color="red">4、Polyphonic Touch PCB Piano - 基于Atmega328P单片机制作的迷你电子琴</font>

来自Hackaday上的一个项目，作者分享了所有的设计文件 - PCB的原理图、布局布线图、Gerber文件（可以直接打板）、直接下载使用的Hex文件以及Arduino的源代码。  

> 项目主页：https://hackaday.io/project/178953-polyphonic-touch-pcb-piano

核心器件采用了Arduino Uno上的经典8位单片机Atmega328P，输入按键采用了触摸按键的方式，没有物理按键，节省了成本，输出声音采用蜂鸣器，并用4个不同的频率合成以达到较好的声音效果。

![](http://henjay724.com/image/biweekly20210530/Polyphonic-Touch-PCB-Piano.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

