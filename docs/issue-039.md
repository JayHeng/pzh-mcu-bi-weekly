# 痞子衡嵌入式半月刊： 第 39 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 38 期》](https://www.cnblogs.com/henjay724/p/15173788.html)

## 唠两句

后天是白露，历史上的今天：1983年9月5日，中国最大的城市引水工程 - 引滦入津工程正式通水。

本期共收录 1个资讯、4个项目、1个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、知名媒体 Aspencore 主办的“全球 MCU 生态发展大会” 落幕</font>

8月26日由 Aspencore 主办的全球 MCU 生态发展大会在深圳圆满落幕，这次会议以“把握「芯」基建，共绘MCU生态”为主题，汇聚了众多微控制器领域的技术和应用专家，共同探讨最新处理器技术、边缘AI、新兴应用和生态发展等热门议题。

> 演讲议程： https://www.eet-china.com/techevents/MCU.html#section04

此次会议国内一众 MCU 厂商都参加了，包括兆易创新、极海半导体、国民技术、华大半导体、灵动微电子、沁恒微电子、雅特力等，各大厂商都分别介绍了自己家的产品发展路线，其中兆易创新即将推出的 GD32H 系列 800MHz 主频产品让人印象最深刻。  

![](http://henjay724.com/image/biweekly20210905/Aspencore-GD32H.PNG)

## 项目类

### <font color="red">1、EVM - 一款通用、精简的超轻量物联网虚拟机</font>

EVM 全称 Embedded Virtual Machine，本质上是一款通用、精简的嵌入式虚拟机，由语法解析前端框架和字节码运行后端构成，可运行在资源受限制的单片机上。

> 项目主页： https://github.com/scriptiot/evm

EVM 优势特点：

```text
1. 纯C开发、零依赖、跨平台、内置REPL；
2. 最小编译体积50KB，最小内存占用2KB;
3. 支持多语言混合开发;
4. 先进的内存管理，无内存泄露和内存碎片问题;
5. 灵活的虚拟机扩展技术，多语言可共享扩展功能;
```

![](http://henjay724.com/image/biweekly20210905/EVM.PNG)

### <font color="red">2、blinker-library - 一套跨硬件、跨平台的物联网解决方案</font>

Blinker 是一套跨硬件、跨平台的物联网解决方案，提供APP端、设备端、服务器端支持，使用公有云服务进行数据传输存储。可用于智能家居、数据监测等领域，可以帮助用户更好更快地搭建物联网项目。Blinker 当前支持 Arduino, ESP8266, ESP32 平台。

> 项目主页： https://github.com/blinker-iot/blinker-library

### <font color="red">3、LittleD - 为嵌入式设备和传感器节点设计的关系型数据库</font>

LittleD 是为嵌入式设备和传感器节点设计的关系型数据库，提供一个 SQL 前端来管理关系模型的数据。

> 项目主页： https://github.com/graemedouglas/LittleD

LittleD 是专为 Arduino Mega2560 这些设备所专门设计的。LittleD 支持表创建，数据插入和 SELECT-FROM-WHERE 语法。LittleD 也支持错误信息，但不是强制性的。一个简单的配置头部文件可以指定编译的特性，所以可以根据应用的需求控制数据库代码脚本。

### <font color="red">4、IonDB - 用于资源受限系统的键值数据库</font>

IonDB 专为 Arduino 和 IoT 提供开箱即用的，基于磁盘的快速存储功能，为受限系统提供键值存储功能，速度非常快，可以充分提升 Arduino 的性能。

> 项目主页： https://github.com/iondbproject/iondb

一般情况下，IonDB 支持：
```text
1. 存储一个键的任意值
2. 重复键支持
3. 范围和等值查询
4. 基于硬盘的持久化数据存储
```

## 工具类

### <font color="red">1、USB-HID-TEST - 轻量级 USB 调试工具</font>

USB-HID-TEST 是 jakey 大神用 python2.7、Tkinter、pywinusb(pyusb-linux) 模块开发的 USB 调试工具。  

> 工具主页： https://gitee.com/jakey.chen/USB-HID-TEST

![](http://henjay724.com/image/biweekly20210905/USB-HID-TEST.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

