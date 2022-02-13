# 痞子衡嵌入式半月刊： 第 49 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 48 期》](https://www.cnblogs.com/henjay724/p/15837047.html)

## 唠两句

立春是上周五的事，这个嵌入式半月刊也坚持到第三年了，离当初定下的 100 期目标已经快完成过半了。

痞子衡祝各位读者在 2022 虎年里工作顺利，事业有成，爱情甜蜜，家庭幸福，专业技术突飞猛进，成为行业专家。

本期共收录 2个资讯、3个项目、1个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、英伟达并购ARM案告吹，ARM谋求IPO</font>

持续一年多时间、备受各方关注的英伟达收购ARM案最终告吹。据CNBC消息，当地时间2月8日，英伟达在联合发布的一份新闻稿中表示，由于“重大监管挑战”，英伟达从软银收购ARM的计划已经失败。

软银集团还宣布，他们将与 Arm 进行协调，将在于 2023 年 3 月 31 日结束的财年内开始准备 Arm 的公开募股事宜。软银集团相信，Arm 的技术和知识产权将继续成为移动计算和人工智能开发的核心。

> * 资讯来源：https://blogs.nvidia.cn/2022/02/09/nvidia-and-softbank-group-announce-termination-of-nvidias-acquisition-of-arm-limited/

### <font color="red">2、智芯半导体发布第二个产品家族Z20K148</font>

近日，中国专业汽车级芯片供应商 - 智芯半导体，推出基于Arm Cortex M4F的汽车级微控制器Z20K148，主要面向汽车车身控制、功能网关，智能座舱、新能源BMS、电机控制等多种应用。

> * 产品主页：https://www.zhixin-semi.com/product?productid=61f34e4d219b6b640f115bed

ZC20K148采用业界领先的40nm生产制造工艺，主频高达160MHz，通过AEC-Q100认证，按照ISO26262流程开发，满足ASIL-B。Z20K148的AUTOSAR MCAL, SDK，评估板，参考设计陆续上线。

![](http://henjay724.com/image/biweekly20220213/zhixin_Z20K148.PNG)

## 项目类

### <font color="red">1、wolfSSL - 一个轻量级的嵌入式SSL/TLS加密库</font>

wolfSSL 是一个基于C语言的轻量级 SSL/TLS 库，专门针对嵌入式和 RTOS 环境，主打特点是体积小，速度快，功能集。

wolfSSL 的起源可追溯到2004年，当时Larry Stefonic和Todd Ouska意识到没有其他开源，双重授权的嵌入式SSL库可用。OpenSSL当时是可用的，但许多OpenSSL用户想要一个可以轻松便携，更小，更快，在明确的商业许可下可用的替代方案，配备了一个干净而现代的 API，并提供商业风格的开发人员支持。

> * 项目地址：https://github.com/wolfSSL/wolfssl

![](http://henjay724.com/image/biweekly20220213/wolfSSL.PNG)

### <font color="red">2、wolfBoot - 一种开源的商用级嵌入式bootloader</font>

wolfBoot 是一种可移植的，与操作系统无关的安全引导加载程序解决方案，它依靠 wolfCrypt 进行固件身份验证，并提供固件更新机制。

> * 项目地址：https://github.com/wolfSSL/wolfBoot

wolfBoot 支持多个密钥库和/或基于硬件的公共密钥加速器，例如Freescale-LTE和STM32-PKA。通过与wolfTPM的集成提供了TPM-2.0支持。wolfBoot 不执行任何特定的密钥配置，在最简单的情况下，只需创建一个私钥并使用它为目标签名更新。

![](http://henjay724.com/image/biweekly20220213/wolfBoot.PNG)

### <font color="red">3、QueueForMcu - 用于单片机的队列功能模块</font>

QueueForMcu 是一个基于单片机实现的队列功能模块，主要用于8位、16位、32位非运行RTOS的单片机应用，兼容大多数单片机平台。

> * 项目地址：https://github.com/xiaoxinpro/QueueForMcu

QueueForMcu 主要特点：

```text
1. 动态创建队列对象
2. 动态设置队列数据缓冲区
3. 静态指定队列元素数据长度
4. 采用值传递的方式保存队列数据
```

## 工具类

### <font color="red">1、MCU_Font - LVGL的多语言转换工具</font>

如果你的项目用到了LVGL，然后需要中英文切换，官方提供了转换工具（https://lvgl.io/tools/fontconverter） ， 不过需要有字库，而且操作起来非常复杂。

LVGL默认提供的字库是非常大，它是英文及字符全量的库，非常庞大，非常耗资源。这时候你可以试试 MCU_Font 软件，它可以按需生成对应的字库。中英文，甚至日语，韩语，图标全部能混搭使用，非常方便的一个工具。

> * 软件地址：https://gitee.com/WuBinCPP/MCU_Font_Release

![](http://henjay724.com/image/biweekly20220213/MCU_Font.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

