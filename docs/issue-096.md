# 痞子衡嵌入式半月刊： 第 96 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 95 期》](https://www.cnblogs.com/henjay724/p/18079011)

## 唠两句

历史上的今天：

本期共收录 3 个项目，2 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、CHERIoT RTOS - 面向嵌入式安全物联网的RTOS</font>

CHERI 的全称是 Capability Hardware Enhanced RISC Instructions，硬件增强 RISC 指令，由英国剑桥大学与美国 SRI International 的合作研究项目。

CHERIoT（用于物联网的RISC-V功能硬件扩展）建立在 CHERI 和 RISC-V 之上，提供 ISA 和软件模型，让依赖于对象粒度空间的软件在内存释放后具有确定性和安全性，直接暴露给 C/C++ 语言模型的轻量级划分。这可以在全新的RTOS上运行现有的嵌入式软件组件，该 RTOS 可扩展到大量隔离（安全通信）空间，即使在SRAM低于256 KB的系统上也是如此。

 * 项目地址：https://github.com/Microsoft/cheriot-rtos

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-096/SOF.PNG)

### <font color="red">2、SOF - 一个开源的音频数字信号处理(DSP)固件</font>

Sound Open Firmware (SOF) 是一个开源的音频数字信号处理(DSP)固件基础设施和SDK。SOF 作为一个社区项目提供基础设施、实时控制部件和音频驱动程序。

 * 项目地址：https://github.com/thesofproject/sof

SOF 固件和 SDK 适用于对现代 dsp 上的音频或信号处理感兴趣的开发人员。SOF 提供了一个框架，音频开发人员可以在其中创建、测试和调整以下内容:

```text
- 音频处理管道和拓扑。
- 音频处理组件。
- DSP基础设施和驱动程序。
- 主机操作系统基础设施和驱动程序。
```

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-096/SOF.PNG)

### <font color="red">3、hoard-of-bitfonts - 包含大量旧式电脑上使用的位图字体</font>

随着操作系统和 gui 转向可伸缩的矢量字体，在20世纪80年代和90年代占主导地位的位图字体在不明显的二进制格式中逐渐消失，并迅速陷入默默无闻。这个存储库的主要目的是将这些位图字体从二进制的束缚中解放出来，保留单色位图排版的古老艺术以供人类欣赏。

 * 项目地址：https://github.com/robhagemans/hoard-of-bitfonts

## 工具类

### <font color="red">1、HexEd.it - 一款在线的Hex编辑器</font>

HexEd.it 是完全免费的商业和非商业用途的 Hex 编辑器，无需安装即可在所有现代浏览器中运行。

 * 软件主页：https://hexed.it/

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-096/HexEd-it.PNG)

### <font color="red">2、FreeType - 一个开源软件字体引擎</font>

FreeType 是一个免费提供的软件库，用于渲染字体。它是用 C 语言编写的，设计成小巧、高效、高度可定制和可移植的，同时能够生成大多数矢量和位图字体格式的高质量输出(字形图像)。

 * 软件主页：https://freetype.org/

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-096/FreeType.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

