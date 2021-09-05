# 痞子衡嵌入式半月刊： 第 38 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 37 期》](https://www.cnblogs.com/henjay724/p/15116438.html)

## 唠两句

明天是处暑，历史上的今天：961年8月22日，宋太祖赵匡胤 “杯酒释兵权”，罢去禁军将领及地方藩镇的兵权，加强了中央集权。

本期共收录 6个项目，希望对你有帮助！

## 项目类

### <font color="red">1、AWTK - ZLG 开发的开源 GUI 引擎</font>

AWTK 全称 Toolkit AnyWhere，是 ZLG 开发的开源 GUI 引擎，旨在为嵌入式系统、WEB、各种小程序、手机和 PC 打造的通用 GUI 引擎，为用户提供一个功能强大、高效可靠、简单易用、可轻松做出炫酷效果的 GUI 引擎。

> 项目主页： https://github.com/zlgopen/awtk

![](http://henjay724.com/image/biweekly20210822/awtk.PNG)

### <font color="red">2、CodeBrick - 一种无OS的MCU实用软件管理系统</font>

CodeBrick 是一种无OS的MCU实用软件框架，包括任务轮询管理，命令管理器、低功耗管理、环形缓冲区等实用模块。系统中广泛利用自定义段技术减少各个模块间的耦合关系，大大提供程序的可维护性。

> 项目主页： https://gitee.com/moluo-tech/CodeBrick

主要功能：

```text
- 支持模块自动化管理，并提供不同优先等级初始化声明接口。
- 支持任务轮询管理，通过简单的宏声明即可实现，不需要复杂的声明调用。
- 支持低功耗管理，休眠与唤醒通知。
- 支持命令行解析，命令注册与执行。
- blink设备支持，统一管理LED、震动马达、蜂鸣器
```

### <font color="red">3、mini-T12 - 基于Arduino平台Atmege328p的条形焊台</font>

mini-T12 是开源条形焊台项目，15Hz PWM输出，DCDC-LDO二级降压电源，板载温度芯片作冷端补偿，内置曲线拟合校准功能，休眠，屏保。

> 项目主页： https://gitee.com/Lichengjiez/mini-T12

![](http://henjay724.com/image/biweekly20210822/miniT12-1.PNG)

![](http://henjay724.com/image/biweekly20210822/miniT12-2.PNG)

### <font color="red">4、MiniDSO-Pro - B站老刘示波器Pro版本</font>

B站老刘示波器Pro版本，在原版的基础上，扩展了测量负电压的功能，更新了UI设计，屏幕升级为1.3寸OLED屏。

> 项目主页： https://gitee.com/zeweni/mini-dso-pro

![](http://henjay724.com/image/biweekly20210822/MiniDSO-Pro-1.PNG)

![](http://henjay724.com/image/biweekly20210822/MiniDSO-Pro-2.PNG)

### <font color="red">5、XS40 - 一款小巧的80键分体键盘</font>

XS40 是80键分体键盘，采用非常便宜的单片机（新唐的N76E003）和USB HID接口芯片（南京沁恒CH9328），目的就是打造一款低成本的机械键盘DIY方案。

> 项目主页： https://gitee.com/play565/XS40

![](http://henjay724.com/image/biweekly20210822/XS40.PNG)

### <font color="red">6、XUAN-Bike - 自动驾驶自行车</font>

B站大佬稚晖君出品，这款自动驾驶自行车不仅会直行、拐弯、躲障、上路，还配备了特斯拉都没有的激光雷达，最终硬件成本不到一万。

> 项目主页： https://github.com/peng-zhihui/XUAN

![](http://henjay724.com/image/biweekly20210822/XUAN.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

