# 痞子衡嵌入式半月刊： 第 51 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 50 期》](https://www.cnblogs.com/henjay724/p/15973021.html)

## 唠两句

昨天是惊蛰，历史上的今天：1973年3月27日，《教父》获第45届奥斯卡最佳影片等3项大奖。

本期共收录 2个资讯、3个项目、1个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、Keil MDK新增完全免费的Community版本</font>

最近，Keil 官方推出了 MDK-Community 版（之前 MDK-Lite 的升级版），该版本有很多国内开发者很在意的特点：免费且没有代码大小限制。这个社区版可供业余爱好者、创客、学生以及学术界人士作为评估使用。MDK-Community 版不限制代码大小并可支持所有非商业应用场景。  

> * 资讯来源：https://www.keil.com/pr/article/1299.htm

![](http://henjay724.com/image/biweekly20220327/Keil_MDK_Community.PNG)

### <font color="red">2、微软正式推出VS Code嵌入式插件</font>

早在 2021 年底微软就宣布 VS2022 预览版将支持嵌入式编程，近日微软发布了基于 VS Code 的嵌入式开发插件（Embedded Tools），支持Azure RTOS、FreeRTOS操作系统。这个插件尚处于早期版本，支持嵌入式 MCU 这方面的功能可能相对要弱一点，当然，基本的功能肯定是有的，比如：调试、断点、查看寄存器等功能。  

> * 资讯来源：https://devblogs.microsoft.com/cppblog/vscode-embedded-development/

![](http://henjay724.com/image/biweekly20220327/vsc_embedded_tools.png)

![](http://henjay724.com/image/biweekly20220327/vscode_embedded.png)

## 项目类

### <font color="red">1、TinyUF2 - 面向 UF2 文件格式的 Bootloader</font>

TinyUF2 主要针对使用 TinyUSB 协议栈的 MCU，目前支持ESP32-S2、i.MXRT10xx、LPC55xx、STM32F4。使用 UF2 bootloader，可以方便的通过 USB 以磁盘模式更新程序，无需其它软件，非常方便。

> * 项目地址：https://github.com/adafruit/tinyuf2

### <font color="red">2、libinimini - 适用单片机的 ini 极简解析库</font>

市面上大多数 ini 解析库几乎都涉及到了 fopen()/fgets().. 以及 malloc()，所以主要适用于 linux 系统。libinimini 是一个非常简单的 ini 配置文件解析库，适用于 RTOS 或裸跑的单片机。

> * 项目地址：https://github.com/lovemengx/libinimini

libinimini 具有以下几种特点：

```text
1. 内存空间占用可控，libinimini 只使用用户指定的一段内存空间进行解析和返回结果。
2. 不关心数据的来源，libinimini 通过回调用户的接口获取每一行文本，不关心文本来自文件还是其它通信接口。
3. 使用方便简单易上手，用户只需实现以行为单位的文本数据回调接口，之后只需等待 libinimini 解析结果即可。
```

### <font color="red">3、heatshrink - 面向嵌入式领域的超小型压缩库</font>

heatshrink 是基于 LZSS 的小型压缩库，声称使用 50-300 字节的内存可以很好地运行。支持压缩和解压，没有版权设置，随意使用。Flash需求方面，作者用avr-gcc测试，仅需1KB的空间。

> * 项目地址：https://github.com/atomicobject/heatshrink

heatshrink 与 gzip 性能比较：

![](http://henjay724.com/image/biweekly20220327/heatshrink.PNG)

## 工具类

### <font color="red">1、Renode - 嵌入式平台的开源模拟器</font>

Renode 是一个用于嵌入式平台的开源仿真器。它支持 x86(Intel Quark)、 Cortex-A (NVIDIA Tegra)、 Cortex-M、 SPARC (Leon)和基于risc-v 的平台。Renode 不仅可以模拟 CPU指令，还可以模拟外设，甚至可以模拟板载的外设。

> * 软件官网：https://renode.io/

![](http://henjay724.com/image/biweekly20220327/Renode.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

