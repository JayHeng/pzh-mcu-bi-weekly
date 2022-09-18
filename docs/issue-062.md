# 痞子衡嵌入式半月刊： 第 62 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 61 期》](https://www.cnblogs.com/henjay724/p/16690371.html)

## 唠两句

历史上的今天：。

本期共收录 1 个项目、0 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、Lua-RTOS-ESP32 - 基于Lua语言面向嵌入式的RTOS</font>

Lua RTOS 是一个实时操作系统，设计在嵌入式系统上运行，对 FLASH 和 RAM 内存的要求最低。目前 Lua RTOS 可用于 ESP32, ESP8266 和 PIC32MZ 平台，并可以轻松移植到其他32位平台。  

> * 项目主页：https://github.com/whitecatboard/Lua-RTOS-ESP32

Lua RTOS 有 3 层设计:

```text
- 在顶层有一个Lua 5.3.4解释器，它为程序员提供Lua编程语言提供的所有资源，以及用于访问硬件的特殊模块(PIO、ADC、I2C、RTC等)，以及Lua RTOS提供的中间件服务(Lua Threads、LoRa WAN、MQTT等)。
- 中间层是一个由FreeRTOS驱动的实时微内核。这就是事情在预期时间内发生的责任。
- 底层是硬件抽象层，它与平台硬件直接通信。
```

![](http://henjay724.com/image/biweekly20220918/Lua-RTOS-ESP32.PNG)

## 工具类



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

