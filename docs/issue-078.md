# 痞子衡嵌入式半月刊： 第 78 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 77 期》](https://www.cnblogs.com/henjay724/p/17438279.html)

## 唠两句

历史上的今天：。

本期共收录 2 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、LiteX - 高效创建FPGA内核/soc的基础框架</font>

LiteX 框架提供了一个方便和高效的基础设施来创建 FPGA 内核/ soc，探索各种数字设计架构和创建完整的基于FPGA的系统。

> * 项目地址：https://github.com/enjoy-digital/litex

LiteX提供了轻松创建 FPGA 核心/SoC 所需的所有常见组件:

![](http://henjay724.com/image/biweekly20230628/LiteX2.PNG)

基于 VexRiscv-SMP CPU 的多核 Linux SoC, LiteDRAM, LiteSATA与LiteX构建并集成，运行在廉价的重新利用的Acorn CLE215+采矿板上：

![](http://henjay724.com/image/biweekly20230628/LiteX.PNG)

### <font color="red">2、xiotman - 一套解决物联网终端应用多样化挑战的软件架构</font>

xiotman 是一套致力于解决物联网终端应用多样化挑战的软件架构解决方案。目前默认的仓库代码下，主要支持了 app_uart_debug 应用，和 app_smart_room 应用（基于RA4M2），其他demo应用还在进一步完善中。

xiotman 的特点：

```text
- 应用的多样性：支持多应用开发
- 组件的多样性：支持多组件解耦
- RTOS的多样性：支持多RTOS
- MCU的多样性：支持多MCU
```

> * 项目地址：https://github.com/recan-li/xiotman

![](http://henjay724.com/image/biweekly20230628/xiotman.PNG)

## 工具类

### <font color="red">1、JI2C - 一款能直接读写芯片寄存器的USB转I2C模块上位机</font>

JI2C 是 Jooiee 出品的一款能直接读写芯片寄存器的USB转I2C模块以及上位机解决方案，可以自定义批量读写，支持中断触发，生成读曲线。

> * 工具官网：http://jooiee.com/cms/ruanjian/112.html

![](http://henjay724.com/image/biweekly20230628/JI2C.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

