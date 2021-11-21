# 痞子衡嵌入式半月刊： 第 43 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 43 期》](https://www.cnblogs.com/henjay724/p/15418226.html)

## 唠两句

明天是小雪，历史上的今天：1983年11月21日，中国第一台亿次巨型计算机 - “银河—Ⅰ”通过国家鉴定。

本期共收录 3个项目、1个工具，希望对你有帮助！

## 项目类

### <font color="red">1、libjpeg - 广泛使用的 JPEG 编解码库</font>

libjpeg是一个完全用C语言编写的库，包含了被广泛使用的JPEG解码、JPEG编码和其他的JPEG功能的实现。这个库由独立JPEG工作组维护。

> * 项目源码：http://www.ijg.org/files/

### <font color="red">2、FatFs - 面向小型嵌入式系统的 FAT 文件系统</font>

FatFs 是日本的大牛工程师 ChaN 开发的面向小型嵌入式系统的一种通用的 FAT 文件系统，它完全是由 AISI C 语言编写并且完全独立于底层的 I/O 介质。因此它可以很容易地不加修改地移植到其他的处理器当中，如 8051、 PIC、 AVR、 SH、 Z80、 H8、 ARM 等。 FatFs 支持 FAT12、 FAT16、FAT32 等格式。

> * 项目主页：http://elm-chan.org/fsw/ff/00index_e.html

FatFs 程序结构如下图，用户应用程序需要由用户编写，想实现什么功能就编写什么的程序，一般我们只用到 f_mount()、 f_open()、f_write()、 f_read()就可以实现文件的读写操作。底层设备可以是 SD 卡/ATA/USB/NAND/RTC 等。

![](http://henjay724.com/image/biweekly20211121/FatFs.PNG)

### <font color="red">3、LittlevGL - 功能强大且易于使用的嵌入式 GUI 库</font>

LittlevGL 是一个开源免费的GUI，常用于 MCU 级别的设备，支持触摸屏操作，移植简单方便，开发者一直在不断完善更新。

> * 项目主页：https://github.com/lvgl/lvgl

LittlevGL 自带了丰富的控件：窗口、按键、标签、list、图表等，还可以自定义控件；支持很多特效：透明、阴影、自动显示隐藏滚动条、界面切换动画、图标打开关闭动画、平滑的拖拽控件、分层显示、反锯齿、仅耗少量内存的字体等等。

![](http://henjay724.com/image/biweekly20211121/LittlevGL.gif)

## 工具类

### <font color="red">1、IDA Pro - 大名鼎鼎的交互式反汇编工具</font>

IDA Pro 是目前最棒的一个静态反编译软件，其已经成为事实上的分析敌意代码的标准，也是攻击研究领域的重要工具。

> * 软件官网：https://hex-rays.com/ida-pro/

作为反汇编程序的 IDA Pro 能够创建其执行映射，以符号表示（汇编语言）显示处理器实际执行的二进制指令。IDA Pro 可以从机器可执行代码生成汇编语言源代码，并使这些复杂的代码更具人类可读性(这个可读具有相对性)。

![](http://henjay724.com/image/biweekly20211121/IDAPro.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

