# 痞子衡嵌入式半月刊： 第 57 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 56 期》](https://www.cnblogs.com/henjay724/p/16391479.html)

## 唠两句

历史上的今天：1998年6月25日，微软公司发布 Microsoft Windows 98 操作系统。

本期共收录 1个资讯、4个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、恩智浦发布全新MCX微控制器产品组合</font>

恩智浦半导体 NXP Semiconductors 近日正式发布全新的MCX微控制器产品组合，旨在推动智能家居、智能工厂、智慧城市以及许多新兴工业和物联网边缘应用领域的创新。

> * 资讯来源：https://www.nxp.com.cn/company/about-nxp/nxp-debuts-new-mcx-portfolio-of-microcontrollers-for-the-next-era-of-advanced-industrial-and-iot-edge-computing:NW-NXP-DEBUTS-NEW-MCX-PORTFOLIO-OF-MICROCONTROL

全新MCX微控制器(MCU)产品组合包含四大全新产品系列，基于通用平台构建，受到恩智浦广泛采用的MCUXpresso开发工具和软件套件支持，可简化产品开发：

![](http://henjay724.com/image/biweekly20220625/NXP-MCX.PNG)

## 项目类

### <font color="red">1、Somu - 基于STM32L432设计的安全密钥小产品</font>

Somu 是一个很小的 FIDO2 安全密钥，你可以用它与谷歌、Twitter和GitHub账户进行双重认证，或者用它与微软账户进行无密码登录。 Somu适合你的USB接口，所以你再也不会忘记你的钥匙。

> * 项目主页：https://solokeys.com/collections/all/products/somu-tiny-security-key-two-factor-authentication-u2f-and-fido2-usb-a

![](http://henjay724.com/image/biweekly20220625/somu.PNG)

Somu 具体规格包括：

```text
- Supported Protocols: FIDO2, U2F
- Supported Operating Systems: Linux, Microsoft Windows, Mac OS X, Chrome OS
- Supported Browsers: Chrome, Firefox, Edge, and Safari support is coming soon (GA in MacOS Catalina)
- Secure Processor: STM32L432KC (with TRNG, security isolation for keys, two levels of locked flash)
- Crypto Algorithms: ECC P256 (as per FIDO2 standard)
- Host Interface: USB-A
- Interaction: two touch buttons - in our FIDO2 firmware the two buttons behave as a single one
- Feedback: RGB LED
- Size: 0.5 x 0.5 x 0.1 inches (13 x 13 x 2.4 mm)
- Weight: 0.11 ounces (3 g)
```

### <font color="red">2、Minimal printf - Mbed推出的精简 printf 实现</font>

鉴于 C 标准库里的 printf 实现比较占空间，Mbed 自己造了个 Minimal printf 库。

> * 项目主页：https://github.com/ARMmbed/mbed-os/tree/master/platform/source/minimal-printf

下面是一个基于恩智浦 K64 的裸机工程在 MDK，GCC 和 IAR 平台下 Flash 以及 RAM 空间占用比较：

![](http://henjay724.com/image/biweekly20220625/Minimal-printf.PNG)

### <font color="red">3、Black Magic Probe - 开源的标准 GNU 调试器</font>

Black Magic Probe 是一个现代的在应用程序调试工具。用户可以使用GNU源代码级调试软件GDB精确地控制发生的事情。 串行线输出(SWO)允许目标器在不使用usb或串口的情况下向主机写入跟踪和日志记录。 在探针中解码SWO本身使得SWO的查看就像连接到串口一样简单。 

> * 项目主页：https://github.com/blackmagic-debug/blackmagic

![](http://henjay724.com/image/biweekly20220625/Black-Magic.PNG)

### <font color="red">4、ctxLink - 面向Cortex-M的无线调试器</font>

ctxLink 是基于 Black Magic Probe（BMP）的开放式硬件，开放式固件调试开发板，支持WiFi连接和电池供电的操作。它实现了SWD和JTAG接口，用于ARM Cortex-M微控制器的远程无电缆编程和调试。

> * 项目主页：https://www.crowdsupply.com/sid-price/ctxlink

![](http://henjay724.com/image/biweekly20220625/ctxLink.PNG)

```text
易用性
- 基于BMP的开放式硬件和开源固件
- 使用内置的STM32系统引导加载程序进行固件更新
- 与Windows，Mac和Linux兼容
调试
- 实现SWD和JTAG接口
- 支持广泛的ARM Cortex目标，包括ST，Atmel，Nordic，NXP等
- 包括一个内置的GDB服务器，可以与各种集成开发环境（IDE）一起使用
- 支持多种目标电压（1.7 V至5 V）
连接性
- 支持与主机的USB和Wi-Fi连接
- 可以使用WPS或通过智能手机的HTTP设置来配置Wi-Fi
功率
- 可以从目标电源供电（仅3 V至5 V目标）
- 可以由LiPo电池（不包括在内）供电。已通过Adafruit的3.7V 1200mAh电池进行测试
- 电池可以通过USB充电
- 无论ctxLink本身是由电池供电还是通过USB供电，均可用于为目标供电（最大100 mA）
```

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

