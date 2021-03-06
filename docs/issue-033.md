# 痞子衡嵌入式半月刊： 第 33 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 32 期》](https://www.cnblogs.com/henjay724/p/14827850.html)

## 唠两句

上周六是芒种，历史上的今天：2011年6月13日，达拉斯小牛队4:2击败三巨头热火，第一次夺得NBA总冠军，诺维茨基获NBA总决赛MVP。

本期共收录 2条资讯、5个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、英特尔拟收购RISC-V阵营领头厂商SiFive</font>

据外媒路透社报道，英特尔正计划以 20 亿美元的价格收购加州半导体初创公司 SiFive。SiFive 成立于 2015 年，是全球首家基于 RISC-V 架构的半导体企业，最新估值在 5 亿美元左右。

众所周知，英特尔是主导x86架构芯片技术的业界龙头，在「三分天下」的处理器架构格局中，英特尔希望通过收购 SiFive，将第三大架构 RISC-V 也收入囊中。

![](http://henjay724.com/image/biweekly20210613/Intel_RISC-V.PNG)

谈判尚处早期阶段，SiFive 也面对着其他多家公司的收购意向，最终可能仍保持独立。

### <font color="red">2、Keil发布新一代开发工具 - Keil Studio</font>

Keil Studio 是 Keil 去年就开始预热的下一代开发工具。近日 Keil 公布了其第一个组件 Keil Studio Cloud（beta版评测），这是一个基于浏览器的IDE，可用于IoT、ML和嵌入式开发。

> 资讯主页：https://www.keil.com/pr/article/1295.htm

![](http://henjay724.com/image/biweekly20210613/Keil_Studio_Cloud.PNG)

首批加入Keil Studio Cloud评测的三款 MCU 平台均出自痞子衡的东家恩智浦：

![](http://henjay724.com/image/biweekly20210613/Keil_Studio_Cloud_HW.PNG)

## 项目类

### <font color="red">1、LibU - 支持多平台的 C 语言程序库</font>

LibU 是一个支持多平台的 C 语言程序库，包含很多独立的模块，例如：内存分配、网络和URI解析、字符串处理、调试和日志记录，LibU 是一个很小的库，差不多只有 70K 左右。这是一个模块化的，支持多平台，包括嵌入式平台的程序库。

> 项目主页：https://github.com/koanlogic/libu

### <font color="red">2、microseconds - MCU通用微秒(us)计时函数框架</font>

microseconds 是一种非常简单实用的通用计时函数框架，这个框架的目的是统一计时函数接口，并且在实现上将通用部分和硬件相关部分剥离开，这样嵌入式项目在使用这个框架时可以无缝快捷地切换底层定时器。

> 项目主页：https://github.com/JayHeng/microseconds

microseconds 提供的实用 API 接口包括：

```C
//! @brief 获取定时器时钟源数值
uint32_t microseconds_get_clock(void);
//! @brief 获取系统累计计数值
uint64_t microseconds_get_ticks(void);
//! @brief 将计数值转换为时间值(微秒)
uint32_t microseconds_convert_to_microseconds(uint64_t ticks);
//! @brief 将时间值(微秒)转换为计数值
uint64_t microseconds_convert_to_ticks(uint32_t microseconds);
//! @brief 阻塞型延时(微秒级)
void microseconds_delay(uint32_t us);
//! @brief 设置超时时间（用于非阻塞型延时）
void microseconds_set_delay(uint32_t us);
//! @brief 判断是否超时（用于非阻塞型延时）
bool microseconds_is_timeout(void);
```

### <font color="red">3、RunTiny - 基于ATtiny10仅778字节实现的跑步小游戏</font>

RunTiny 是一个国外小哥设计的基于 AVR ATtiny10 以及 128x32 单色 OLED 的跑步者小游戏，代码和硬件设计文件全部开源。

> 项目主页：https://github.com/ridoluc/RunTiny

为了能够将代码塞到 1KB 的 Flash 存储器里面，作者做了优化，全部用汇编语言写成，最终的代码只有778个字节，不仅实现了游戏的功能，也处理了 MCU 的 I/O 与显示屏的通信（基于TWI接口协议）。

![](http://henjay724.com/image/biweekly20210613/RunTiny.gif)

### <font color="red">4、ESP32-Smart-Watch  - 基于ESP32 WROOM的开源智能手表</font>

这个项目是一个完全开放源码的基于 ESP32 WROOM 模块实现的智能手表，完成度非常高。项目设计里串行通信和充电完全通过板载micro usb接口，无需任何外部接口板处理。

> 项目主页：https://github.com/Bellafaire/ESP32-Smart-Watch

固件分为 V1 和 V2 两版，V1偏低功耗设计，需要触摸唤醒使用；V2是全功能设计，仅轻度睡眠，可用加速度计唤醒。

![](http://henjay724.com/image/biweekly20210613/ESP32-Smart-Watch.PNG)

### <font color="red">5、Macro Mechanical Keypad  - 6键超迷你键盘DIY</font>

一个国外小哥写的超详细教程，教我们制作一个由 Arduino 控制的 6 键小键盘。

通过这个教程，我们可以学习到：完成一个小键盘需要什么，如何组装，如何编程，以及如何改进或自己独立创新。

> 教程主页：https://www.instructables.com/Custom-Macro-Mechanical-Keypad/

![](http://henjay724.com/image/biweekly20210613/Macro-Mechanical-Keypad.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

