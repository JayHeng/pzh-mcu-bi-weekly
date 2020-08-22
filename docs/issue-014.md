# 痞子衡嵌入式半月刊： 第 14 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 13 期》](https://www.cnblogs.com/henjay724/p/13455615.html)

## 唠两句

今天是处暑。

本期共收录 条资讯、个项目、个工具、1个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、智芯云联合ST、瑞兴恒方同步发行LoRaWAN® OpenCPU评估板TSC_WL_EVK</font>

近日，深圳智芯云联合意法半导体(STM)、腾讯TenentOSTiny团队、瑞兴恒方同步发行基于TencentOS Tiny开源物联网操作系统的LoRaWAN® OpenCPU评估板TSC_WL_EVK。

![](http://henjay724.com/image/biweekly/TSC_WL_EVK.png)

TSC_WL_EVK评估板板载瑞兴恒方(RisingHF)出品的的高集成度RHF0M0E5 LoRa模组，模组整体体积只有12x12x2.5mm，外围电路简单，外设接口丰富便于开发者根据项目要求进行灵活配置。评估板集成了物联网俱乐部兼容的E53扩展接口，可以外接所有兼容E53接口的传感器扩展板。

借助腾讯云TencentOSTiny物联网开源操作系统，可以让开发者快速上手体验TencentOS Tiny基础内核和最新的LoRaWAN物联网组网技术。能帮助客户进一步节省资源，降低开发成本和BOM成本，优化系统功耗，让物联网产品开发更加便捷，加速终端产品的落地和推向市场。

## 项目类

### <font color="red">1、tinyriscv - 一个极简易懂的RISC-V处理器核</font>

tinyriscv 是网友 liangkangnan 设计并维护的一个从零开始写的极简、非常易懂的RISC-V处理器核。作者从事的是嵌入式软件相关的工作，做这个项目的初衷是为了入门RISC-V，熟悉RISC-V的指令内容和汇编语法。

> 项目地址： https://gitee.com/liangkangnan/tinyriscv

tinyriscv 是一个单核32位的小型RISC-V处理器核，采用verilog语言编写，设计目标是对标ARM Cortex-M3系列处理器。tinyriscv 在 Xilinx Artix-7 35T FPGA 平台(时钟50MHz)上运行CoreMark跑分成绩为2.4。其整体框架如下：

![](http://henjay724.com/image/biweekly/tinyriscv_arch.PNG)

tinyriscv 有以下特点：

```text
1. 支持RV32IM指令集，通过RISC-V指令兼容性测试；
2. 采用三级流水线，即取指，译码，执行；
3. 可以运行C语言程序；
4. 支持JTAG，可以通过openocd读写内存(在线更新程序)；
5. 支持中断；
6. 支持总线；
7. 支持FreeRTOS；
8. 支持通过串口更新程序；
9. 容易移植到任何FPGA平台(如果资源足够的话)；
```


## 工具类

### <font color="red">1、</font>



## i.MXRT出品

### <font color="red">1、迈瑞医疗 - 注射泵BeneFusion nVP</font>

这款注射泵是行业突破产品，7寸全触摸彩屏，SafeDose药品管理系统有效消除药品混淆错误，创新的SmartAIR系统确保更精确地检测气泡，革命性的SmartRapid系统确保2秒通电、4秒装填、3秒内送完第一滴。配合临床辅助应用InfusionView系统使医务人员能够在患者监护仪屏幕上查看输液数据。

> * RT芯片：i.MXRT1052
> * 产品系列主页： https://www.mindray.com/cn/productlist/products_line71.html
> * 参考售价： 未知

![](http://henjay724.com/image/biweekly/Mindary_BeneFusion_nVP.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


