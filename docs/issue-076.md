# 痞子衡嵌入式半月刊： 第 76 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 75 期》](https://www.cnblogs.com/henjay724/p/17300090.html)

## 唠两句

历史上的今天：。

本期共收录 4 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、USB-C Power Supply - 基于STM32F091的USB-C电源</font>

国外小伙 Andrew 建立的一个简单的电源项目，以此来获得一些相对较新的USB电源传输(USB- pd)技术的实际操作经验。USB-PD 允许通过接口提供高达20V的电压和高达5A的电流。小伙分享了全部设计细节，可以让我们深入了解 USB-PD 的工作原理。

这个电源主控为意法 STM32F091，测量前端 ADC 使用得德州仪器 INA233，PD 控制器是意法 STUSB4500。

> * 项目主页：https://circuitcellar.com/research-design-hub/basics-of-design/build-a-usb-c-power-supply/

![](http://henjay724.com/image/biweekly20230430/USB-C-PowerSupply.PNG)

### <font color="red">2、LogicAnalyzer - 基于树莓Pico开源逻辑分析仪</font>

此项目是一个非常便宜的基于树莓Pico逻辑分析仪。该分析仪提供多达24个数字通道，前置和后触发采样，边缘触发和模式触发高达16位。

最基本的版本是纯Pico，只需要短接GPIO0和GPIO1，上传固件就可以了。当然，这有一些限制，因为Pico只支持3.3v，如果想用它来诊断5v信号，需要配套一个电平转换板。

除了硬件之外，该逻辑分析仪还包括一个功能强大的软件(目前仅限Windows)，可以在其中可视化捕获的数据，导出捕获，使用协议分析器等。

> * 项目主页：https://github.com/gusmanb/logicanalyzer

![](http://henjay724.com/image/biweekly20230430/LogicAnalyzer0.PNG)

![](http://henjay724.com/image/biweekly20230430/LogicAnalyzer1.PNG)

### <font color="red">3、moteus - 四足机器人开源BLDC电机控制器</font>

moteus 无刷控制器可以将业余无刷电机转变为高性能伺服执行器。它集成了必要的驱动电子设备，高性能32位微控制器（STM32G4），绝对磁编码器和高速数据接口在一个紧凑的封装。电源和数据是菊花链集成到多个伺服系统。

> * 项目主页：https://github.com/mjbots/moteus

![](http://henjay724.com/image/biweekly20230430/moteus.PNG)

### <font color="red">4、RasPico_SHIBAKI_Board - 基于树莓Pico实现超低成本的双光纤网卡100BASE-FX</font>

该项目通过树莓派的可编程 I/O 来实现以太网 MAC，软件硬件全开源。

> * 项目主页：https://github.com/kingyoPiyo/RasPico_SHIBAKI_Board

![](http://henjay724.com/image/biweekly20230430/RasPico_SHIBAKI_Board.PNG)

## 工具类

### <font color="red">1、得捷电子实时展示芯片厂家供货周期</font>

得捷电子官网专门开辟了一个页面实时展示主流芯片厂家供货周期。

> * 工具官网：https://www.digikey.cn/zh/resources/reports/lead-time-trends

![](http://henjay724.com/image/biweekly20230429/digikey-LeadTimeTrends2.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

