# 痞子衡嵌入式半月刊： 第 109 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 108 期》](https://www.cnblogs.com/henjay724/p/18444618)

## 唠两句

历史上的今天：1999年10月14日，中国发射第一颗传输型对地遥感资源卫星 - “资源一号”。

本期共 4 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、RAMTEX - 适用于RGB/多级灰度/黑白屏的GUI</font>

RAMTEX 是一家软件公司，专注于黑白/RGB/多级灰度屏的图形用户界面（GUI）开发，他们的 GUI 框架为市面上大部分的 LCD 驱动器都做了适配。此外他们还做了一系列测试工具（PC 上模拟器，字库编辑软件，还有一套能在 PC 上快速调试各种 LCD 屏的软硬件）。  

 * 项目地址：https://www.ramtex.dk/

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-109/RAMTEX-1.PNG)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-109/RAMTEX-2.PNG)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-109/RAMTEX-3.PNG)

其中 IOTester 将“嵌入式”I/O硬件连接到 PC，并使硬件可以直接从用 C 或 c++ 编写的普通 PC 程序应用程序访问和控制。

### <font color="red">2、canopen - ECSS组织创建的适用于航天器的CANopen</font>

该项目是 ECSS（(European Cooperation for Space Standardization，欧洲空间标准化合作组织）创建的一个适用于航天器的 CANopen 版本，提供完整的 CANopen 软件栈实现，符合 CiA 301， CiA 306 和 ECSS-E-ST-50-15C 标准，针对关键嵌入式系统的高度可定制和可配置的开源库。

 * 项目地址：https://gitlab.com/n7space/canopen

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-109/canopen.PNG)

### <font color="red">3、ecat_servo - 基于STM32的EtherCAT CiA402伺服驱动</font>

EtherCAT 是用于自动化的实时以太网协议，目前最流行的 EtherCAT 伺服驱动应用协议是 CANopen（基于EtherCAT） CiA402。该项目是 CoE CiA402 标准的开源实现，用于开放式电机控制器，如 ODrive， STMBL 等。该项目展示了如何使用免费和开源工具进行 EtherCAT 设备开发。

 * 项目地址：https://github.com/kubabuda/ecat_servo

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-109/ecat_servo.PNG)

### <font color="red">4、programmable_precision_resistor - 一个开源可编程精密电阻仪</font>

该项目是一个纯开源的可编程电阻仪，其电阻值可以通过数字信号来调节，可调范围 1Ω - 999.999KΩ，支持 SCPI 可编程仪器标准命令。

 * 项目地址：https://github.com/sbstnh/programmable_precision_resistor

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-109/programmable_precision_resistor.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

