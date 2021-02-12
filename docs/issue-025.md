# 痞子衡嵌入式半月刊： 第 25 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 24 期》](https://www.cnblogs.com/henjay724/p/14322190.html)

## 唠两句

立春是上周三的事了，很抱歉推迟了近10天才给大家带来新一期半月刊，大家放心，半月刊有可能会迟，但绝不会缺席。

今天是牛年大年初一，痞子衡就给大家拜个年吧，祝各位读者在牛年里工作顺利，事业有成，爱情甜蜜，家庭幸福，专业技术突飞猛进，成为行业大牛。

本期共收录 2条资讯、2个项目、2个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、瑞萨电子推出Arm Cortex MCU产品家族全新RA4M2 MCU产品群，扩展在低功耗工业与物联网应用中的覆盖范围</font>

> 产品主页:  https://www2.renesas.cn/ra4m2?utm_campaign=mcu_ra4m2&utm_source=press_release&utm_medium=press_release&utm_content=ra4m2

近日， 瑞萨电子宣布推出12款全新RA4M2微控制器（MCU）产品，以扩展其RA4系列MCU阵容。新产品将超低功耗、高性能和增强的安全性充分结合，使其成为工业与物联网应用的理想解决方案。 

![](http://henjay724.com/image/biweekly/RA4M2.jpg)

RA4M2 MCU产品群的关键特性：

```text
- 提供运行模式下80μA/MHz的超低功耗，唤醒时间为30μs
- 采用100MHz主频Arm Cortex-M33内核，支持TrustZone技术
- 包含瑞萨安全加密引擎的完整安全解决方案
- 提供48-100引脚LQFP封装，以及48引脚QFN封装
- 集成512KB、384KB或256KB闪存，128K SRAM
- 电容式触摸感应单元
- 全速USB 2.0
- 高级模拟功能，支持一路ADC
- QuadSPI
- SDHI
```

RA4M2 MCU采用基于Armv8-M架构的Arm® Cortex®-M33内核，集成Arm TrustZone®技术和瑞萨安全加密引擎。安全加密引擎包含多个对称和非对称加密加速器、高级密钥管理、安全的生命周期管理、抵抗功率分析攻击和篡改检测功能。这一组合使客户能够实现安全芯片功能，让物联网边缘设备等低功耗应用获得安全保障。

### <font color="red">2、瑞萨正式收购Dialog，为车用芯片业务市场积极布局</font>

2月8日，据瑞萨电子最新公告宣布，瑞萨与电源管理提供商Dialog已就以每股67.50欧元全现金方式收购Dialog全部已发行股本和将要发行股本的条款达成协议，总股权价值约为49亿欧元（约合59亿美元）。收购完成后，Dialog将成为瑞萨电子的全资子公司，这为瑞萨在车用芯片市场的竞争注入新的活力。

![](http://henjay724.com/image/biweekly/Dialog_Renesas.png)

> 芯片主页：https://www.dialog-semiconductor.com/press-releases/renesas-and-dialog-semiconductor-join-forces-advance-global-leadership-embedded

尽管2021年汽车芯片市场供不应求，但并不妨碍半导体巨头收购动作频现。瑞萨电子在汽车微控制器领域拥有约30%的全球市场份额，车用芯片约占其营收的一半。Dialog以其低功耗和混合信号专业技术为核心，拥有非常广泛且丰富的产品系列，包括电池和电源管理、电源转换、CMIC、LED驱动器、ASIC、无线充电技术等，是高集成度和高能效混合信号IC的重要供应商，为物联网、消费电子产品以及汽车和工业终端市场的高增长细分市场中的众多客户提供服务。两家公司技术资产的互补性和产品组合的规模将使瑞萨电子能够构建更强大、更全面的解决方案，以服务于物联网和汽车市场等高增长细分市场。

## 项目类

### <font color="red">1、key_board - 用于单片机中的小巧多功能按键支持库</font>

key_board 是网友 wei513723 维护的用于单片机中的小巧多功能按键支持库。

> 项目主页: https://gitee.com/wei513723/key_board

软件采用了分层的思想，并且做到了与平台无关，用户只需要提供按键的基本信息和读写io电平的函数即可，非常方便移植，同时支持多个矩阵键盘及多个单io控制键盘，目前已实现按下触发、弹起触发、长按自动触发、长按弹起触发、多击触发、连续触发等功能，并且能够随意组合（支持状态的同一时间轴和非同一时间轴），后续还会添加更多的功能。

### <font color="red">2、WATCH-X - 一款功能丰富的智能手表</font>

WATCH-X是一款基于LittleVGL的开源智能手表项目, 能够支持高质量流畅(60FPS+)的动画效果的显示，炫酷的界面加上易于扩展的系统框架，非常容易上手，下面是WATCH-X展示的部分功能UI界面。

> 工具主页：https://github.com/FASTSHIFT/WatchX

![](http://henjay724.com/image/biweekly/Watch-X.png)

WATCH-X能够支持功能主要有9大类，分别是时间显示，温度显示，气压显示，海拔显示，秒表，亮度控制，时间控制，简易游戏系统，自动关机等。为支持这些功能需求，硬件系统如下：

```text
* 1.主控: STM32F411CEU6 (主频:100MHz RAM:128KB ROM:512KB)
* 2.屏幕: ST7789 IPS 1.14inch SPI接口 135x240分辨率 100Hz刷新率
* 3.输入设备: 按键x3
* 4.RTC:MCU内置RTC时钟
* 5.加速度计:MPU6050
* 6.气压计:BMP180
* 7.电源管理:TP4056 + TPS63070
```

该手表项目还提供了详细的硬件原理图设计文件和PCB设计文件作为参考，轻松就能玩转起来！

## 工具类

### <font color="red">1、SQLite - 强大的适用于多平台的SQL数据库引擎 </font>

SQLite是世界上部署最广泛的数据库，它是一种C语言库，它实现了一个小型，快速，自包含，高可靠性，功能齐全的SQL数据库引擎。

> 项目主页: https://www.sqlite.org/index.html

![](http://henjay724.com/image/biweekly/SQLite.jpg)

SQLite是嵌入式SQL数据库引擎。与大多数其他SQL数据库不同，SQLite没有单独的服务器进程。SQLite直接读取和写入普通磁盘文件。数据库文件格式是跨平台的，用户可以在32位和64位系统之间或在big-endian和 little-endian 体系结构之间自由复制数据库 。这些功能使SQLite成为应用程序文件格式的流行选择。

SQLite是一个紧凑的库。启用所有功能后，库大小可以小于600KB，具体取决于目标平台和编译器优化设置。在内存使用和速度之间需要权衡。SQLite通常为您提供的内存越多，运行速度就越快。但是，即使在低内存环境下，性能通常也相当不错。根据使用方式，SQLite可以比直接文件系统I/O更快。

### <font color="red">2、sqlcipher - 适用于本地数据存储的更加安全的SQLite</font>

SQLCipher扩展了SQLite项目，以添加安全性增强功能，使其更适合于加密的本地数据存储，例如：动态加密，篡改检测，内存清理，强密钥派生等。SQLCipher基于SQLite，并且稳定地集成了稳定的上游发行功能。

> 项目主页: https://github.com/sqlcipher/sqlcipher

SQLCipher具有如下的功能特点：

```text
- 高性能，许多操作的加密开销仅为5-15％
- 数据库文件的100%加密
- 良好的安全模式（CBC模式，HMAC，密钥派生）
- 零配置和应用级加密
```

SQLCipher也与标准SQLite数据库兼容。如果未提供密钥，则SQLCipher的行为将与标准SQLite库类似。使用ATTACH和sqlcipher_export（）便捷函数，也可以从纯文本数据库（标准SQLite）转换为加密的SQLCipher数据库。

感兴趣的嵌入式er可以去尝试在自己的设备上使用sqlcipher 及SQLite。

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

