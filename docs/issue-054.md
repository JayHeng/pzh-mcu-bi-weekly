# 痞子衡嵌入式半月刊： 第 54 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 53 期》](https://www.cnblogs.com/henjay724/p/16167075.html)

## 唠两句

明天是谷雨，历史上的今天：1989年5月3日，卡内基·梅伦大学研制出无人驾驶汽车。

本期共收录 1个资讯、2个项目、0个工具、1个 RT 产品，希望对你有帮助！

## 资讯类

### <font color="red">1、ARM公司发布Cortex-M85内核</font>

近日 Arm 发布了新一代的 Cortex-M 处理器，Cortex-M85。简单说：Cortex-M85 ≈ Cortex-M7 + TrustZone + Helium（Cortex-M版本的NEON)，最大特色：支持Helium可以通过SIMD指令集提供强大的DSP性能。

> * 资讯主页：https://www.arm.com/company/news/2022/04/arm-expands-total-solutions-for-iot-portfolio

![](http://henjay724.com/image/biweekly20220503/Cortex-M85.PNG)

## 项目类

### <font color="red">1、STMBL - 基于STM32F4的开源伺服驱动器</font>

STMBL 是一款开源伺服驱动器，专为 CNC 机床和机器人改造而设计。它支持高达 320V 和 2kW 的工业交流和直流伺服。软硬件已经升级了好几个版本（目前最新版本 v4.1），主控是 STM32F4 系列，所有资料齐全。

> * 项目主页：https://github.com/rene-dev/stmbl

![](http://henjay724.com/image/biweekly20220503/STMBL.PNG)

### <font color="red">2、CortexProg - 半开源Cortex-M下载器</font>

CortexProg 可用于给 Cortex-M 内核芯片下载程序。分为两大版本，早期版本基于 ATTiny85，这个版本是全开源的，但是由于性能有限，最新版本采用 EFM32 来实现。最新版本上位机是开源的，而 EFM32 的程序仅提供了固件，没有提供源码，但是用户可以通过上位机扩展新的芯片支持。  

> * 项目主页：https://cortexprog.com/

![](http://henjay724.com/image/biweekly20220503/CortexProg.PNG)

![](http://henjay724.com/image/biweekly20220503/CortexProg_VS.PNG)

## 工具类


## i.MXRT出品

### <font color="red">1、索尼 - 2022新一代游戏电视(XR-X90K)</font>

索尼XR-X90K系列是一款性价比极高的液晶电视。创新设计解锁更多技能；智能化操作无须看管更加放心；简洁大方的外观设计也让人一见倾心；便携的操作和使用体验给繁忙的生活挤出了多点的时间去感受和享受，让懒人也能有道。

> * RT芯片：i.MXRT1011
> * 产品主页： https://www.sonystyle.com.cn/products/bravia/x90k/xr_75x90k.html
> * 官网定价： 6999 元起

![](http://henjay724.com/image/biweekly20220503/Sony_XR-75X90K.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

