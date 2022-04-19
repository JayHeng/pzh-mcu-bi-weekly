# 痞子衡嵌入式半月刊： 第 53 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 52 期》](https://www.cnblogs.com/henjay724/p/16103152.html)

## 唠两句

明天是谷雨，历史上的今天：1971年4月19日，苏联用质子号运载火箭将世界上首个太空站礼炮1号送上太空。

本期共收录 3个项目、1个工具、2个 RT 产品，希望对你有帮助！

## 项目类

### <font color="red">1、EventOS - 超级轻量、事件驱动型嵌入式开发框架</font>

EventOS 包含两个项目，分别是 EventOS Nano 和 EventOS Basic。

EventOS Nano 是一个面向单片机、事件驱动的嵌入式开发平台。它主要有两大技术特色：一是事件驱动，二是超轻量。EventOS Nano 目标是开发一个企业级的嵌入式开发平台，以事件总线为核心，打造一个统一的嵌入式技术生态，为广大企业用户和嵌入式开发者们，提供搞可靠性的、高性能的、现代且高开发效率的嵌入式开发环境。

> * 项目主页：https://gitee.com/event-os/eventos

EventOS Basic 是一个超级简洁的协作式内核。它的特点有二：一是协作式，不抢占，按优先级轮询，当前任务不释放CPU控制权，其他任务得不到CPU，二是超级轻量（ROM 968字节，RAM 64字节，-O3）。目前提供出来的功能非常基础，主要有两部分，一是任务功能，二是软定时器功能。

> * 项目主页：https://gitee.com/event-os/eventos-basic

### <font color="red">2、AVR-Crypto-Lib - 适用于小内存MCU的开源加密算法库</font>

AVR-Crypto-Lib 是一组不同加密算法实现的合辑。由于微控制器的特殊限制(非常小的空间，RAM和Flash的范围从几个字节到几个KiB)，正常的算法优化实现是不可用的。 因此，AVR-Crypto-Lib 提供特殊的实现，以适用微控制器应用程序的极端有限的资源。

> * 项目官网：https://wiki.das-labor.org/w/AVR-Crypto-Lib/en
> * 项目主页：https://git.cryptolib.org/avr-crypto-lib.git

AVR-Crypto-Lib 虽然于 2015 年已经停止更新，但是对于资源受限的芯片，如果需要加密功能，还是非常合适的。

![](http://henjay724.com/image/biweekly20220419/AVR-Crypto-Lib.PNG)

### <font color="red">3、TI-RSLK - TI公司推出的小车开发套件</font>

TI-RSLK 是一种低成本的机器人工具包和课堂课程，为学生提供了对电子系统设计如何工作的更深入的理解。TI-RSLK 包含多个版本。

TI-RSLK迷宫版（也是第一个版本）课程有20个学习模块，涵盖了基本到高级主题。 每个模块都配有教学视频和幻灯片，实验文档和演示视频，测验和课堂活动。TI-RSLK的目标是教授嵌入式系统和应用程序，并可以扩展和使用在各种工程类。

> * 项目官网：https://university.ti.com/programs/RSLK/

![](http://henjay724.com/image/biweekly20220419/TI-RSLK.PNG)

## 工具类

### <font color="red">1、emWin字体生成器</font>

allyzc 做的一个 emWin 的字体生成器，支持多国文字，支持抗锯齿。用法如下：

```text
1、左侧输入待转换的文字，支持输入多国文字，支持抗锯齿。
2、选择合适的字体和大小。
3、设置字模的高度和偏移与抗锯齿，1表示无抗锯齿。
4、设置编码格式，并输入字体名字。
5、点击开始转换。
6、保存文件或是直接复制代码到C文件。
```

> * 下载链接：https://www.armbbs.cn/forum.php?mod=viewthread&tid=87428

![](http://henjay724.com/image/biweekly20220419/emWIN_char_generator.PNG)

## i.MXRT出品

### <font color="red">1、大疆创新 - 手持云台(如影RONIN-S)</font>

如影Ronin-S是针对单反和微单开发的专业手持云台,轻巧便携可单手操作。载具模式最高速度75公里/小时,载重3.6千克,续航12小时。巨像摄影、定点延时、轨迹延时、轨迹摄像等智能模式让专业拍摄变得简单。

> * RT芯片：i.MXRT1061/1062
> * 产品主页： https://www.dji.com/cn/ronin-s
> * 官网定价： 4399 元起

![](http://henjay724.com/image/biweekly20220419/Ronin-S.PNG)

### <font color="red">2、大疆创新 - 口袋云台相机(灵眸OSMO pocket)</font>

OSMO Pocket 是 DJI 迄今為止最小的相機,輕巧,易攜,並配備獨立螢幕。 1/2.3 英寸傳感器,80°廣角鏡頭,f/2.0 光圈,拍攝 4K/60fps 超高清影片。輕鬆拍攝,記錄生活。

> * RT芯片：i.MXRT600
> * 产品主页： https://www.dji.com/cn/osmo-pocket
> * 官网定价： 2499 元起

![](http://henjay724.com/image/biweekly20220419/OSMO-pocket.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

