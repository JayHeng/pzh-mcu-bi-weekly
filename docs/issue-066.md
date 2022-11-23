# 痞子衡嵌入式半月刊： 第 66 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 65 期》](https://www.cnblogs.com/henjay724/p/16819509.html)

## 唠两句

历史上的今天：1935年11月6日，美国工程师阿姆斯特朗在无线电工程学会纽约分部首次发表文章描述调频广播。

本期共收录 4 个项目、 2 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、AVH-TFLmicrospeech - 基于TFL-M的语音识别包入门</font>

这是 ARM 发布的一个基于 TensorFlow Lite 的语音识别包，程序分析一个音频输入与语音识别模型，可以检测两个关键字- Yes 和 No，然后将识别的关键字打印到串口中。

示例程序既可以在 Arm虚拟硬件(AVH)上执行，也可以在物理硬件目标（i.MXRT1050/1060）上执行。

> * 项目地址：https://github.com/ARM-software/AVH-TFLmicrospeech

### <font color="red">2、ThunderScope - 雷电USB4开源示波器</font>

ThunderScope 是为 Thunderbolt 设计的第一个示波器，允许实时采样数据以超过 1 GB/s 的速度流到计算机。通过利用现代设备强大的处理能力，该设计消除了传统示波器的所有限制。ThunderScope 是完全开源的，所有的开发和设计决策都在其 hackaday 上详细说明。  

> * 项目地址：https://github.com/EEVengers/ThunderScope
> * 项目主页：https://hackaday.io/project/180090-thunderscope

ThunderScope 参数指标：

```text
- Channels: Four
- Analog Bandwidth: 350 MHz
- Sample Rate: 1 GS/s
- Resolution: 8-bit
- Voltage ranges (with 1× probe): 1 mV to 10 V per division
- Memory Depth: As many gigabytes as you can allocate!
```

![](http://henjay724.com/image/biweekly20221106/ThunderScope.PNG)

### <font color="red">3、Aeropoint GUI - 支持通过PPT文件创建界面的GUI方案</font>

Aeropoint GUI 是日本一家叫 CRI WARE 公司的产品，本是面向 PC 端的 GUI 解决方案。但其也推出了 Aeropoint GUI for RX，这是一个特殊版本，使所有基本的 Aeropoint 功能可用于普通的低成本微控制器，比如瑞萨的 RX65N・RZ/A 等。  

Aeropoint GUI 采用出色的色彩还原技术，还可以使用 PowerPoint 创建 GUI、播放音频与视频。

> * 项目主页：https://www.cri-mw.co.jp/business/product/embedded/aeropointguien/

![](http://henjay724.com/image/biweekly20221106/AeropointGUI.PNG)

### <font color="red">4、jsmn - 号称世界上最快的JSON解析器/标记器</font>

jsmn 是基于 C 语言的一个极简的 JSON 解析器，它可以很容易地集成到资源有限或嵌入式项目中。大多数 JSON 解析器提供了一系列函数来加载 JSON 数据、解析数据并根据其名称提取任何值。jsmn 证明了检查每个 JSON 包的正确性或分配临时对象来存储解析的 JSON 字段通常是一种过度的做法。  

> * 项目地址：https://github.com/zserge/jsmn

## 工具类

### <font color="red">1、IAR Build Tools - 用于CI/CD下进行高效构建和测试工具</font>

IAR 为 Arm 提供支持 Linux 和 Windows 安装的 IAR Build tools，进一步扩展了 IAR Systems 提供的自动化构建的灵活自动化工作流。支持在基于跨平台的框架中实现自动化应用程序构建和测试过程，这些工具支持关键软件构建和测试的大规模部署。

> * 项目主页：https://www.iar.com/bxarm

如下是一个 IAR Build Tools、Gitea 和 Jenkins 部署集成设置的方法示例：

![](http://henjay724.com/image/biweekly20221106/IAR-Build-Tools.PNG)

### <font color="red">2、EEZ Studio - 开源跨平台模块化可视化低代码开发工具</font>

EEZ Studio 是一个开源的跨平台(在电子中开发)模块化可视化低代码开发工具和SCPI控制器，适用于 EEZ BB3 T&M 设备和 EEZ H24005 可编程电源和其他 T&M 设备，支持来自Keysight, Rigol, Siglent, Tek/Keithley, R&S 等制造商的 SCPI。

> * 项目主页：https://www.envox.eu/studio/studio-introduction/
> * 项目地址：https://github.com/eez-open/studio

![](http://henjay724.com/image/biweekly20221106/EEZ-Studio.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

