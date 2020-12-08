# 痞子衡嵌入式半月刊： 第 21 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 20 期》](https://www.cnblogs.com/henjay724/p/14021089.html)

## 唠两句

昨天是大雪。

今天的半月刊是史上第二次延期。

本期共收录 2条资讯、0个项目、1个工具、1个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、芯来科技RISC-V处理器家族迎来新成员900系列IP</font>

近日芯来科技发布RISC-V处理器家族新成员 - 900系列IP，该系列处理器具备丰富的配置并支持多种操作系统以满足工业级控制、AI等高性能计算、或交互式图型多媒体应用等多种领域的需求，非常适合对标ARM Cortex-A35，A53，M7，R5等内核。

芯来科技900系列的所有产品均为9级流水线、双发射架构，可通过模块化进行特性组合，方便用户按领域需求定制，其中：

```text
•N900为32位高性能嵌入式和实时控制处理器；
•NX900为64位高性能嵌入式和实时控制处理器；
•UX900为配置内存管理单元（MMU）的64位双模处理器，既可作为支持Linux系统加载的应用处理器，又可作为实时控制处理器。
```

![](http://henjay724.com/image/bi-weekly/nucleisys_900series.PNG)

### <font color="red">2、中国移动首颗MCU芯片CM32M101A发布</font>

中国移动近日正式发布了自己首款MCU芯片CM32M101A，这是一款用于物联网产品的芯片，具有集成度高、低功耗、低成本、高性能接口和加密存储器等几大特点。尤其适用于物联网行业应用，如智能表计、环境监测、智慧家庭、防盗报警、定位器和智能家电等。

![](http://henjay724.com/image/bi-weekly/CM32M101A.png)

CM32M101A具备丰富的片上资源。高达108MHz的内核，可提供较高的计算能力。相对于同价位产品，提供更大更可靠的存储单元。极低的功耗特别适用于物联网终端电池供电的场景。同时芯片具有硬件的安全算法加速模块，可为物联网终端提供更强的安全能力。

## 项目类

### <font color="red">1、</font>




## 工具类

### <font color="red">1、 SerialChart - 能将串口数据实时绘制成波形的软件</font>

SerialChart是由Sergiu Baluta开发的开源软件，它能用于实时绘制通过串行（RS-232）端口接收到的数据。它可以通过插件和WebView javascript集成来支持其他类型的端口。这个软件采用模块化的设计允许受激励的编码器添加新类型的端口、解码器和显示过滤器。

SerialChart基本数据处理流程为：端口（来自串行/USB端口的原始数据）->解码器（处理数据）->值（显示在屏幕/图表上）。

> 下载地址：https://github.com/starlino/serialchart

![](http://henjay724.com/image/biweekly/SerialChart.png)

## i.MXRT出品

### <font color="red">1、野火电子 - fireDAP高速仿真器</font>

fireDAP是一款基于CMSIS DAP深度优化的仿真器，集在线硬件仿真和固件下载功能于一体，免驱动，适用于所有Cortex-M内核的MCU。固件经过深度优化，下载速度稳定，不丢固件，坚如磐石。配套野火独家开发的fireDAP上位机，可实现hex、bin、elf、axf文件的下载，可脱离编译软件操作。

> RT芯片：i.MXRT1011
> 产品主页： https://www.firebbs.cn/forum.php?mod=viewthread&tid=30894&highlight=fireDAP
> 官网定价： 138 元

![](http://henjay724.com/image/cnblogs/fireDAP_view.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


