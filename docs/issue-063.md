# 痞子衡嵌入式半月刊： 第 63 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 62 期》](https://www.cnblogs.com/henjay724/p/16704565.html)

## 唠两句

历史上的今天：。

本期共收录 1 个资讯、3 个项目、0 个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、兆易创新发布GD32A503系列首款车规级MCU</font>

近日兆易创新 GigaDevice 发布首款基于 Cortex®-M33 内核的 GD32A503 系列车规级微控制器，正式进入车规级 MCU 市场。GD32A503 新品采用 40nm 车规级制程和高速嵌入式闪存 eFlash 技术，并通过 DFM 可制造性设计及高测试向量覆盖，实现研发与制造的协同，以提升成品率和可靠性，满足严苛的车用市场需求。  

> * 资讯来源：https://www.gigadevice.com/zh-hans/press-release/gigadevice-launches-gd32a503/

GD32A503 系列 MCU 基于 100MHz Cortex®-M33 内核，配备 384KB Flash 和 48KB SRAM，另有专用代码空间可配置为 64KB DFlash/4KB EEPROM。芯片采用 2.7-5.5V 宽电压供电，工作温度范围 -40~+125℃，工作寿命 15 年以上。GD32A503 产品组合提供了 4 种封装共 10 个型号选择。

![](http://henjay724.com/image/biweekly20220925/GD32A503.PNG)

## 项目类

### <font color="red">1、cola_os - 300行代码实现的多任务管理的OS</font>

cola_os 是一个 300 行代码实现多任务管理的 OS，在很多 MCU 开发中，功能很简单，实时性要求不强，如果使用 RTOS 显得太浪费，任务多了管理不当又很乱，所以 cola_os 这种简单好用的轮询式任务管理是更合适的选择。  

> * 项目主页：https://gitee.com/schuck/cola_os

![](http://henjay724.com/image/biweekly20220925/cola_os.PNG)

### <font color="red">2、TMCM-1617-GRIP-REF - Trinamic推出的开源机械臂参考设计</font>

这是 TMCM-1617 无刷直流伺服驱动器的开源硬件参考设计。为了在机械臂应用中使用，该板设计了标准夹持器电子外形。它能够通过EtherCAT®，IO-Link®，或使用 Trinamic 的 TMCL 协议 RS485 控制无刷直流电机。  

> * 项目主页：https://www.trinamic.com/support/eval-kits/details/tmcm-1617-grip-ref/

![](http://henjay724.com/image/biweekly20220925/TMCM-1617-GRIP-REF-1.PNG)
-
![](http://henjay724.com/image/biweekly20220925/TMCM-1617-GRIP-REF-2.PNG)

### <font color="red">3、QUARK - 全开源的多功能手持测量工具</font>

QUARK 是一个简单、易于使用的多功能开发工具，适用于 Arduino、ESP32、STM32 和类似的平台。它由在Arduino环境中编写的开源软件提供支持, 开发人员也可以修改设备固件来添加功能或修改现有的功能以满足自己的需求。  

> * 项目主页：https://www.crowdsupply.com/mulin/quark

QUARK 开箱即用，可以测量电压、电流、电阻、电容和电感等参数。它还有一个内置示波器，一个 UART 记录器，一个 UART 绘图仪和一个频率发生器。最后，它还可以通过蓝牙将数据发送到自定义的 iOS和Android 应用程序，在那里可以显示和分析数据。

![](http://henjay724.com/image/biweekly20220925/QUARK.PNG)
-
![](http://henjay724.com/image/biweekly20220925/QUARK-2.PNG)

## 工具类


### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

