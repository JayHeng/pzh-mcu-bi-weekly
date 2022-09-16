# 痞子衡嵌入式半月刊： 第 61 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 60 期》](https://www.cnblogs.com/henjay724/p/16567006.html)

## 唠两句

历史上的今天：1956年9月13日，IBM研发成功世界上首个电脑磁盘储存设备。

本期共收录 2 个资讯，3 个项目、1 个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、旗芯微发布最新一代Hyper控制器家族产品FC7300</font>

旗芯微近日发布了最新一代Hyper控制器家族产品，全系列对标英飞凌 TC家族控制器，覆盖智能底盘、功能安全控制器、域控制器等应用领域。超融合HPU（Hyper Processing Unit）FC7300系列芯片的性能媲美英飞凌的TC家族系列，进一步丰富了旗芯微的车规产品家族。  

> * 资讯来源：http://flagchip.com.cn/index.php?c=show&id=75

FC7300产品系列同样基于真5V车规级工艺打造，是基于多个Cortex-M7内核的高性能车规级HPU，并支持高带宽高可靠的片上嵌入式闪存记忆体，支持应用ASIL-D + ASIL-B功能安全等级多核配置，AEC-Q100 认证，Auto-Grade 1等级。  

![](http://henjay724.com/image/biweekly20220910/Flagchip_FC7300.PNG)

### <font color="red">2、兆易创新推出首款自研DDR3L产品GDPxxxLM</font>

兆易创新GigaDevice近日宣布，推出公司首款自研DDR3L产品——GDPxxxLM系列， 提供2Gb/4Gb不同容量选择，实现了从设计、流片，到封测、验证的全流程自主可控，在满足消费类市场强劲需求的同时，兼顾工业及汽车市场应用，可为国产自主供应生态圈的发展构建提供强有力的支撑。  

> * 资讯来源：https://www.gigadevice.com/zh-hans/press-release/gigadevice-launches-the-first-ddr3l/

GDPxxxLM 系列产品采用长鑫存储（CXMT）先进工艺制程，符合 JEDEC 标准，读写速率为2133/1866 Mbps，容量为2Gb/4Gb，支持1.5V和1.35V两种电压。凭借着卓越的性能以及良好的兼容性，GDPxxxLM系列充分满足消费电子产品的主流需求，适用于机顶盒、电视、监控、网络通信、智慧家庭等诸多应用场景，同时也将会针对电力、工业、汽车等行业客户推出工业级颗粒，以满足特定行业市场的需求。  

## 项目类

### <font color="red">1、Open bootloader - ST推出的Bootloader中间件</font>

Open Bootloader是STM32Cube MCU包中提供的应用内编程(IAP)。它与STM32系统引导加载器完全兼容，因此它具有相同的支持接口和命令。它也使用相同的上位机工具，如STM32CubeProgrammer。  

> * 项目主页：https://github.com/STMicroelectronics/stm32-mw-openbl

Open Bootloader 允许所有可能的引导加载程序操作(读，写，擦除，跳转…)到内部(Flash, SRAM, OTP…)或外部内存。Open Bootloader 支持的通信接口包括 USART, I2C, SPI, USB-DFU, FDCAN。

Open Bootloader 支持的命令如下：  

```text
- Get Version
- Get Device ID
- Get Available Command List
- Write Memory
- Read Memory
- Write Protection setting
- Read Protection setting
- Jump to Application
- Flash Erase
- Special Command
- Extended Special Command
```

### <font color="red">2、The battery-free Game Boy - 开源软硬件的无电池供电掌机</font>

这是一种由太阳能和在游戏过程中敲击按钮提供能量的电子游戏机。它是一个橙色的砖块，有一本平装小说那么大，但重量只有1989年发行的第一代任天堂Game Boy游戏机的一半。  

该掌机设计最意思的地方是无电池的情况下，提供了点击按钮搜集能量和太阳能搜集能量。

> * 项目主页：https://www.cnet.com/science/features/the-first-battery-free-game-boy-wants-to-power-a-gaming-revolution/

![](http://henjay724.com/image/biweekly20220913/The-battery-free-Game-Boy.PNG)

### <font color="red">3、LCR Meter AU2019 - 开源LCR表</font>

阻抗(Z)是表征无源电子元件(电阻、电容、电感)的重要参数。要确定阻抗，就必须测量至少两个值(大小和相位)，一般是元件两端的电压和流过该元件的电流。LCR Meter AU2019采用自平衡电桥方法，使用一个简单的运算放大器作为电流/电压转换器(I-V转换器)。这种简单的方法以合理的成本提供了良好的测量精度。它的主要缺点是所使用的运算放大器的性能限制其频率范围在高频。  

> * 项目主页：https://www.elektormagazine.com/labs/remake-lcr-meter

该表的特点如下：

```text
- 测试频率从50Hz到2MHz。
- 4种可能的测试电压(100mV, 200mV, 500mV和1V有效值)。
- 额外的直流极化可达5V的电容器和50mA的电感。
```

![](http://henjay724.com/image/biweekly20220913/LCR-Meter-AU2019.PNG)

## 工具类

### <font color="red">1、Virtual Oscilloscope - 可插入网页设计的虚拟示波器频谱仪插件</font>

这个在线虚拟示波器允许可视化现场声音输入，并掌握如何调整显示。如果你想在自己的网站上嵌入示波器，可以直接复制并粘贴以下html到你的网页上。  

```html
<iframe src="https://academo.org/demos/virtual-oscilloscope/?embedded=true" width="800" height="380"></iframe>
```

> * 工具主页：https://academo.org/demos/virtual-oscilloscope/
> * 工具主页：https://academo.org/demos/spectrum-analyzer/

![](http://henjay724.com/image/biweekly20220913/academo-virtual-oscilloscope.PNG)
-
![](http://henjay724.com/image/biweekly20220913/academo-spectrum-analyzer.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

