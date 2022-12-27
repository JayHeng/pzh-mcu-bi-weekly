# 痞子衡嵌入式半月刊： 第 69 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 68 期》](https://www.cnblogs.com/henjay724/p/16974522.html)

## 唠两句

历史上的今天：。

本期共收录 1 个资讯、3 个项目、2 个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、澎湃微电子S038系列Cortex-M0 MCU创造主频记录200MHz</font>

澎湃微电子日前宣布，其新品 PT32S038 系列 Cortex-M0 MCU 创造了新的工作时钟主频记录，以 200M 的 CPU 主时钟工作频率，大幅超越全球已知 Cortex-M0 MCU，全球主流厂商的 Cortex-M0 MCU 时钟主频通常在 48M~72M，少数公司提供 96M 的产品。

> * 资讯来源：网传

当程序在 PT32S038 的 SRAM 里运行，并且 CPU 主时钟设置为 200M 时，其 CoreMark 能够达到 380 分，已经达到或超过目前国际大厂 Cortex-M4 MCU 的工作性能。

![](http://henjay724.com/image/biweekly20221225/PT32S038.PNG)

## 项目类

### <font color="red">1、mOTA - 一款专为32位MCU开发的OTA组件</font>

mOTA 是一款专为 32 位 MCU 开发的 OTA 组件，组件包含了 bootloader 、固件打包器 (Firmware_Packager) 、固件发送器三部分，并提供了一个基于 STM32F103 和 YModem-1K 协议的案例。

> * 项目地址：https://gitee.com/DinoHaw/mOTA

mOTA bootloader 架构:

![](http://henjay724.com/image/biweekly20221228/mOTA_arch.PNG)

mOTA 固件更新流程:

![](http://henjay724.com/image/biweekly20221228/mOTA_flow.PNG)

### <font color="red">2、crc-lib-c - 一个基于C语言的CRC校验库</font>

crc-lib-c 是一个基于C语言的CRC校验库，包括常用的21个CRC参数模型实现，包含CRC-4/5/6/7/8/16/32。

> * 项目地址：https://github.com/whik/crc-lib-c

### <font color="red">3、tiny-AES-c  - 最小巧可移植的AES算法实现库</font>

tiny-AES-c 是一个用C语言编写的AES ECB、CTR和CBC加密算法的小型可移植实现。这个库是为小代码和简单性而设计的，适用于低内存占用和可移植性比高性能更重要的情况。如果速度是一个问题，可以尝试更复杂的库，例如Mbed TLS, OpenSSL等。

> * 项目地址：https://github.com/kokke/tiny-AES-c

tiny-AES-c 的 API 非常简单:

```C
/* Initialize context calling one of: */
void AES_init_ctx(struct AES_ctx* ctx, const uint8_t* key);
void AES_init_ctx_iv(struct AES_ctx* ctx, const uint8_t* key, const uint8_t* iv);

/* ... or reset IV at random point: */
void AES_ctx_set_iv(struct AES_ctx* ctx, const uint8_t* iv);

/* Then start encrypting and decrypting with the functions below: */
void AES_ECB_encrypt(const struct AES_ctx* ctx, uint8_t* buf);
void AES_ECB_decrypt(const struct AES_ctx* ctx, uint8_t* buf);

void AES_CBC_encrypt_buffer(struct AES_ctx* ctx, uint8_t* buf, size_t length);
void AES_CBC_decrypt_buffer(struct AES_ctx* ctx, uint8_t* buf, size_t length);

/* Same function for encrypting as for decrypting in CTR mode */
void AES_CTR_xcrypt_buffer(struct AES_ctx* ctx, uint8_t* buf, size_t length);
```

## i.MXRT出品

### <font color="red">1、谷歌 - 智能手表Pixel</font>

2022年10月6日，谷歌举行新品发布会，正式发布Pixel Watch智能手表新品。Pixel Watch主要亮点是搭载自家智能手表操作系统Wear OS，同时还集成Fitbit，单次充电可以拥有24小时的续航表现，采用41毫米不锈钢表壳，配备1.6英寸AMOLED显示屏，支持DCI-P3色域，亮度高达1000尼特。

> * RT芯片：i.MXRT595
> * 产品主页： https://store.google.com
> * 官网定价： 349.99 美元起

![](http://henjay724.com/image/biweekly20221228/GooglePixel.PNG)

### <font color="red">2、博能Polar - 智能手表Pacer</font>

Polar Pacer是一款不折不扣的 GPS 跑步手表，它为现代跑步者提供了所有必备功能，同时还为他们提供了必需的专业训练工具，让他们只专心于一件事：跑步。

> * RT芯片：i.MXRT595
> * 产品主页： https://www.polar.com/zh-hans/pacer
> * 官网定价： 199.9 欧元起

![](http://henjay724.com/image/biweekly20221228/PolarPacer.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

