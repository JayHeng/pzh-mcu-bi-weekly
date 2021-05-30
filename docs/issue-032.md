# 痞子衡嵌入式半月刊： 第 32 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 31 期》](https://www.cnblogs.com/henjay724/p/14774980.html)

## 唠两句

上周日(5.23)痞子衡组织了一场苏州做公众号的朋友线下见面会。活动很High，下午组队搞篮球，激烈对抗中距离一下子拉近了；晚上啤酒烧烤小龙虾，玩牌助兴，6个人干掉三箱啤酒。其实痞子衡平时不太喝酒，但是和初次见面的朋友小聚，要想气氛到位，必须推杯换盏，果然人均6瓶酒下去，大家都分享了工作多年来的深刻感悟，这才是聚会的意义。  

下个月中旬痞子衡将会在互推中将这些朋友正式介绍给大家。  

![](http://henjay724.com/image/biweekly20210530/mcu_geek_group2.PNG)

本期共收录 0条资讯、2个项目，0个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、</font>

## 项目类

### <font color="red">1、TraNOR - 2495个晶体管DIY的8位/7MHz的CPU</font>

TraNOR是国外一个叫Dennis Kuschel的哥们做的主频7MHz的8位CPU，还有操作系统并支持I2C和SPI总线，所有设计文件全部开源。

> 项目主页：http://www.mynor.org/tranor

TraNor为100%的分立计算机设计，除了使用现成的ROM、RAM和LCD模块之外，CPU和I/O都是由分立的晶体管组成的 ，4个8位的I/O端口使用了598个晶体管，其它的1897个MOSFETs用来搭建CPU。

作者还开发了一个操作系统，包含了一些有用的API功能，并且还做了支持Linux和Windows的交叉编译器。

![](http://henjay724.com/image/biweekly20210530/TraNOR.PNG)

### <font color="red">2、Polyphonic Touch PCB Piano - 基于Atmega328P单片机制作的迷你电子琴</font>

来自Hackaday上的一个项目，作者分享了所有的设计文件 - PCB的原理图、布局布线图、Gerber文件（可以直接打板）、直接下载使用的Hex文件以及Arduino的源代码。  

> 项目主页：https://hackaday.io/project/178953-polyphonic-touch-pcb-piano

核心器件采用了Arduino Uno上的经典8位单片机Atmega328P，输入按键采用了触摸按键的方式，没有物理按键，节省了成本，输出声音采用蜂鸣器，并用4个不同的频率合成以达到较好的声音效果。

![](http://henjay724.com/image/biweekly20210530/Polyphonic-Touch-PCB-Piano.PNG)

## 工具类



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

