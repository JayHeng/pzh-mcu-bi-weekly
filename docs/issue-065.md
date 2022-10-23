# 痞子衡嵌入式半月刊： 第 65 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 64 期》](https://www.cnblogs.com/henjay724/p/16755687.html)

## 唠两句

历史上的今天：1995年10月23日，英国医生移植世界首例电动心脏。

本期共收录 6 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、ESP-BLE-MESH - 乐鑫开源的蓝牙 mesh 协议栈</font>

ESP-BLE-MESH 是乐鑫开源的蓝牙 mesh 协议栈，已通过蓝牙技术联盟 (SIG) 全功能认证，支持 Bluetooth® Mesh Specification v1.0.1 中规定的所有功能与应用模型。使用 ESP-BLE-MESH 技术，可以和全球不同厂商、不同类型的标准蓝牙 mesh 设备互相通信，协同工作。 

> * 项目主页：https://github.com/espressif/esp-idf/tree/master/components/bt/esp_ble_mesh

### <font color="red">2、zBitsView - 单片机实现多层菜单的屏幕界面</font>

zBitsView 是一个基于单片机实现的多层菜单的屏幕界面。硬件原型：STM32F103C8T6、Nokia 5110屏幕，EC11旋转编码器，但是界面控件理论上不限制屏幕、不限制单片机型号，移植非常方便。  

> * 项目地址：https://github.com/figght/zBitsView

使用 zBitsView 设计菜单界面时只需要定义几个数组。首先定义 RowListTypeDef 类型数组，根据界面数定义数组个数，根据每个界面包含的行元素数定义每个数组的长度。然后定义 ViewListTypeDef 类型数组，定义一个即可，数组长度是界面数决定的。

![](http://henjay724.com/image/biweekly20221023/zBitsView.PNG)

### <font color="red">3、FreeEEG32 - 开源EEG脑电图参考设计</font>

FreeEEG32 是一种可堆叠的，开源的，32通道，24位，sigma-delta，多路采样板，旨在满足科学家和大脑黑客的需求。FreeEEG32 结合了 4 个 8 通道 AD7771，主控是 STM32H7。它足够敏感，可以处理高质量的脑电图数据采集。  

> * 项目主页：https://www.crowdsupply.com/neuroidss/freeeeg32

为了满足 EEG 标准，FreeEEG32 的固件在同时运行所有 32 个通道时优化为每个通道 512SPS。通过堆叠 FreeEEG32 板，可以实现 64-256 通道的同步流。每块板独立地连接到主机，但可以流到相同的软件实例进行大量数据收集。  

![](http://henjay724.com/image/biweekly20221023/FreeEEG32.PNG)

FreeEEG32 与市面上其它 EEG 参考板的比较：

![](http://henjay724.com/image/biweekly20221023/FreeEEG32-2.PNG)

### <font color="red">4、DIY-SMU - 源测量单元DIY</font>

DIY-SMU 作者曾为许多行业领导者(Analogic Test and Measurement group, Teradyne DC instruments group, Zoll和HP Medical)工作过许多直流和交流源/测量仪器，以及许多初创公司和家庭项目。但是 DIY SMU 一直是他最想做的事，终于在他退休后，有时间开发硬件，软件，控制和包装，于是便有了这个全开源的 DIY 项目。

> * 项目主页：http://www.djerickson.com/diy_smu/

![](http://henjay724.com/image/biweekly20221023/DIY-SMU.PNG)

DIY-SMU 功能参数如下：

![](http://henjay724.com/image/biweekly20221023/DIY-SMU-2.PNG)

### <font color="red">5、μSMU - 信用卡大小、USB供电的4象限源测量单元</font>

源测量单元(SMU)，是一种能够同时进行源和测量的电子仪器。它可以精确地施加电压或电流，同时测量精确的电压和/或电流。μSMU 不是要取代精密的 SMU，而是在不需要精确性的，但成本敏感的领域补充 SMU。

> * 项目地址：https://github.com/joeltroughton/uSMU

![](http://henjay724.com/image/biweekly20221023/μSMU.PNG)

μSMU 功能参数如下：

![](http://henjay724.com/image/biweekly20221023/μSMU-2.PNG)

### <font color="red">6、LUNA - 开源USB多功能工具+Amaranth HDL框架</font>

LUNA 是一个使用 FPGA 技术与 USB 一起工作的完整工具包，它能提供硬件、网关和软件来启用 USB 应用程序。可用于监控、破解和开发 USB 设备。  

> * 项目地址：https://github.com/greatscottgadgets/luna

![](http://henjay724.com/image/biweekly20221023/LUNA.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

