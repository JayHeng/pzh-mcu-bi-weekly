# 痞子衡嵌入式半月刊： 第 56 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 55 期》](https://www.cnblogs.com/henjay724/p/16321972.html)

## 唠两句

下周二是夏至，历史上的今天：1999年6月19日，由 Valve 公司制作的经典游戏《反恐精英》（Counter-Strike） 正式在美国发售。

本期共收录 1个资讯、2个项目、0个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、云途推出第二款高端车规级MCU - YTM32B1ME</font>

继去年年底量产 L 系列 MCU 后，今年上半年苏州云途半导体又量产了第二款高端车规级MCU - M系列产品YTM32B1ME，这是目前国内唯一实现量产的基于ARM Cortex-M33的高端32位车规级MCU。

> * 产品主页：https://github.com/smartmx/TFDB

![](http://henjay724.com/image/biweekly20220619/YTM32B1M.PNG)

YTM32B1ME芯片采用行业领先的40nm e-Flash工艺，基于32位车规级ARM Cortex-M33内核，CPU全温域主频高达120MHz，提供1.25MB嵌入式闪存，符合ISO26262的ASIL-B等级要求，可靠性满足AEC-Q100、Grade1标准，信息安全方面支持AES、SHA以及国密SM4等多种加密算法，并提供符合AUTOSAR标准的MCAL。

## 项目类

### <font color="red">1、 RL-USB - 集成在MDK中间件里的USB协议栈</font>

RL-USB 是 ARM 官方提供的 USB 协议栈，DAP-LINK 中的 USB 源码就是采用的RL-USB实现。RL-USB 的最大优势就是简单易用，创建各种类和 USB 复合设备都可以通过 MDK RTE 环境一键添加。

> * 项目主页：https://www.keil.com/pack/doc/mw/USB/html/index.html

![](http://henjay724.com/image/biweekly20220619/RL-USB.PNG)

RL-USB 协议栈特点包括：

```text
1. RL-USB支持USB Host和USB Device。
2. RL-USB可以同时管理芯片的多个USB外设。
3. USB Host支持的类：HID，CDC，MSC，自定义类。
4. USB Device支持的类：HID，CDC，MSC，ADC和自定义类。
5. 支持多线程和线程安全操作。
6. 通过MDK的RTE开发环境可以一键添加。
7. 使用MDK基于对话框的配置向导，可以很方便的完成MDK的配置。
```

### <font color="red">2、 TFDB - 超轻量的可纠错的通用单片机flash存储方案</font>

不同于其他很多的KV型数据库，TinyFlashDB 为每一个需要存储的变量都会分配一个单独的单片机flash扇区，变量长度不可变。所以TinyFlashDB仅适用于存储几个关键性变量（例如：IAP跳转标志、系统断电时间等等），不适合大规模数据存储。

> * 项目主页：https://github.com/smartmx/TFDB

TinyFlashDB在设计时就考虑了写入错误的影响，追求力所能及的安全保障、资源占用方面尽可能的缩小（不到1kb代码占用）、尽可能的通用性（可以移植到51等8位机，无法逆序写入的stm32L4系列，某些flash加密的单片机和其他普通32位机上）。


## 工具类



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

