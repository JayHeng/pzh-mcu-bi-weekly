# 痞子衡嵌入式半月刊： 第 53 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 52 期》](https://www.cnblogs.com/henjay724/p/16103152.html)

## 唠两句

明天是谷雨，历史上的今天：1971年4月19日，苏联用质子号运载火箭将世界上首个太空站礼炮1号送上太空。

本期共收录 2个项目、0个工具，希望对你有帮助！

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

## 工具类



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

