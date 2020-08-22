# 痞子衡嵌入式半月刊： 第 14 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 13 期》](https://www.cnblogs.com/henjay724/p/13455615.html)

## 唠两句

今天是处暑。

本期共收录 1条资讯、2个项目、1个工具、1个RT产品，希望对你有帮助！

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

### <font color="red">2、FlashDB - 一款超轻量级嵌入式数据库</font>

FlashDB 是一款超轻量级的嵌入式数据库，专注于提供嵌入式产品的数据存储方案。与传统的基于文件系统的数据库不同，FlashDB 结合了 Flash 的特性，具有较强的性能及可靠性。并在保证极低的资源占用前提下，尽可能延长 Flash 使用寿命。

> 项目地址： https://github.com/armink/FlashDB

FlashDB 提供两种数据库模式：

```text
- 键值数据库 ：是一种非关系数据库，它将数据存储为键值（Key-Value）对集合，其中键作为唯一标识符。KVDB 操作简洁，可扩展性强。
- 时序数据库 ：时间序列数据库 （Time Series Database , 简称 TSDB），它将数据按照 时间顺序存储 。TSDB 数据具有时间戳，数据存储量大，插入及查询性能高。
```

FlashDB 主要特性如下：

```text
1. 资源占用极低，内存占用几乎为 0 ;
2. 支持 多分区，多实例 。数据量大时，可细化分区，降低检索时间；
3. 支持 磨损平衡 ，延长 Flash 寿命；
4. 支持 掉电保护 功能，可靠性高；
5. 支持 字符串及 blob 两种 KV 类型，方便用户操作；
6. 支持 KV 增量升级 ，产品固件升级后， KVDB 内容也支持自动升级；
7. 支持 修改每条 TSDB 记录的状态，方便用户进行管理；
```

## 工具类

### <font color="red">1、TortoiseGIT - 一个Git版本控制系统的Windows客户端</font>

作为一个软件开发人员，不可能不知道Git。Git作为一个复杂的版本控制系统，命令之多，即使经常使用，一些命令也记不住，一般只记住几个常用的命令。TortoiseGit是Windows用户一致推荐的客户端，用GUI（图形界面）方式来操作Git，并且它还是开源的。

> 软件官网： https://tortoisegit.org/

装好TortoiseGit后，软件便会自动识别PC上的所有Git仓库，并标示仓库下各文件状态。使用TortoiseGit特别简单，在仓库文件夹上右击选择对应Git命令即可。

![](http://henjay724.com/image/biweekly/TortoiseGit_cmds.PNG)

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


