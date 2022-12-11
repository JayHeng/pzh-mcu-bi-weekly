# 痞子衡嵌入式半月刊： 第 68 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 67 期》](https://www.cnblogs.com/henjay724/p/16920757.html)

## 唠两句

历史上的今天：1572年12月11日，丹麦天文学者第谷发现了仙台星座中的一颗新星。他以"新星"为题写了一篇论文发表出来。这篇论文胜过一枚巨型炸弹，它动摇了人们一直墨守不疑的亚里士多德的天体不变的学说。

本期共收录 5 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、USB Cable Tester - 各种接口类型USB电缆的便携测试仪</font>

网友 alvarop 制作的一块板卡，能够测试各种 USB 线是否完好。(注意USB标准有助于识别板卡上的这些USB- c，符合标准的电缆将根据电缆和连接器规格发布选择合适的引脚)。将测试的 USB 线连接到板子两侧，如果对应线是通的，那板子上的信号 LED 将被点亮。

> * 项目地址：https://github.com/alvarop/usb_c_cable_tester

![](http://henjay724.com/image/biweekly20221211/usb_c_cable_tester.PNG)

### <font color="red">2、ECBM - 基于STC8系列的外设函数库</font>

ECBM 工作室为 STC8 单片机设计的外设函数库（当前是 V3 版本），目前已经支持 STC8 全型号，外设部分会逐渐完善。STC8 是目前 51 单片机里最好用的系列，拥有最多 8K 的SRAM、64K 的Flash、5个定时器、4个串口。全系列都带IIC和SPI，大部分带ADC。STC8H还带有硬件USB。

ECBM 工作室在推广 ECBM 库 V3 的过程中，用户反馈 ECBM 占用空间太大，新手对库不了解不知道怎么优化，于是、专门推出官方优化精简版！在保证了 ecbm 特色的情况下，去除大量用不到的鸡肋功能，只为了核心和精简而存在的STC8库。

> * 项目地址1：https://gitee.com/ecbm/ecbm_library
> * 项目地址2：https://gitee.com/ecbm/ecbm-library-lite

### <font color="red">3、modbus - 全新可裁剪的modbus协议实现</font>

ECBM 工作室推出的全新的、可裁剪的 modbus 实现。他们的宣传口号是“一定是你没见过的版本，易移植易上手，大量注释让你爱不释手”。该项目在 Gitee 上有 200 多 star。

> * 项目地址：https://gitee.com/ecbm/modbus

### <font color="red">4、ETP - 入门级时间片轮询程序框架</font>

ETP 是 Ecbm-Timeslice-Polling 的缩写，是 ECBM 工作室推出的时间片轮询程序框架。时间片轮询是一种基础框架，可以通过合理地分割任务来充分利用CPU。但ETP并不是实时操作系统，在实际应用中也会出现阻塞，需要根据实际需求来决定如何应用。

> * 项目地址：https://gitee.com/ecbm/timeslice-polling

ETP 具有如下几个特点：

```text
- 任务的优先级固定。所有任务按安装时的顺序执行，不可在运行时更改。
- 任务是静态的，不能在运行时创建、删除。但是可以开启和停止任务。
- 代码不和硬件关联，方便移植。
- 任务之间不会抢占CPU，如果某个任务阻塞，那么整体都会卡主。
- 由于任务按顺序执行，但如果某一任务的执行时间太长，会影响到其他任务的正常运行。
```

### <font color="red">5、BP3621&BP3622 - 面向超薄紧凑型充电设备的无线充电器模块</font>

ROHM 公司开发的具有集成天线板的紧凑型无线充电模块:BP3621(发射器)和BP3622(接收器)。该模块允许将无线电源功能添加到较小的设备，如智能标签/卡或PC外围设备。

> * 发射器：https://www.rohm.com/products/wireless-charger-modules/1356mhz-wireless-charger-modules/bp3621-product#productDetail
> * 接收器：https://www.rohm.com/products/wireless-charger-modules/1356mhz-wireless-charger-modules/bp3622-product#productDetail

BP3621(发射器)和BP3622(接收器)的尺寸各为20mm2至30mm2，采用了优化的天线(线圈)布局。它可以配置一个紧凑的无线充电系统，使用13.56MHz频段提供高达200mW的功率。

![](http://henjay724.com/image/biweekly20221211/BP3621-BP3622.PNG)

![](http://henjay724.com/image/biweekly20221211/BP3621-BP3622-2.PNG)

## 工具类

### <font color="red">1、USBDriveLog - USB驱动器的日志显示小软件</font>

USBDriveLog 是一款适用于 Windows 10 和 Windows 11 的工具，它可以显示插入计算机的所有 USB 驱动器的日志。对于每个u盘事件，显示以下信息:设备型号，修订，制造商，序列号，插拔时间，拔插时间，设备ID，设备容量等。

> * 工具地址：https://www.nirsoft.net/utils/usb_drive_log.html

![](http://henjay724.com/image/biweekly20221211/USBDriveLog.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

