# 痞子衡嵌入式半月刊： 第 19 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 18 期》](https://www.cnblogs.com/henjay724/p/13866420.html)

## 唠两句

今天是立冬。传统是以“立冬”作为冬季的开始，“春生、夏长、秋收、冬藏”，冬季是享受丰收、休养生息的季节。

近期意法半导体(ST)欧洲工厂闹大罢工，罢工原因主要是工厂员工今年没有得到加薪，他们觉得自己不受管理层重视。罢工带来的后果是STM32芯片供货周期受影响，并且部分通用型号涨幅明显（2-3倍）。STM32在国内的高性价比替代品非常多，不少替代品甚至都是Pin2Pin兼容的，这次罢工受益最大的恐怕是这些国产MCU厂商了。

本期共收录 1条资讯、4个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、兆易创新推出GD32E501系列CM33内核MCU，持续布局光模块市场</font>

近日兆易创新推出GD32家族基于Arm® Cortex®-M33内核的最新成员GD32E501系列增强型微控制器。新产品为提高光电传输领域的国产化水平持续开辟道路，强化与现有的GD32E232系列产品的无缝升级并形成应用组合，以匹配光网络各种传输速率和应用场景，全面覆盖光纤路由器、交换机、5G传输、数据中心、云服务器等各类光模块市场的数据处理和监测需求。

> 资讯主页: http://www.gd32mcu.com/cn/detail/306

![](http://henjay724.com/image/biweekly/GD32E501.PNG)

## 项目类

### <font color="red">1、cJSON - 一款基于C语言的轻量级JSON解析库</font>

JSON是一种轻量级的数据交换格式，可以把JSON的结构理解成无序的、可嵌套的key-value键值对集合，这些key-value键值对以结构体或数组的形式来组织的。cJSON是C语言写的一个JSON解析库。

> 项目主页: https://github.com/DaveGamble/cJSON

为什么选择cJSON来解析JSON字符串？因为简洁又简单，而且效率又快，cJSON工程文件也非常简单，仅一个.c文件和一个.h文件！cJSON实际上使用一个双链表来记录JSON数据，然后对这个双链表进行增删改查等操作。

### <font color="red">2、TencentOS-tiny - 腾讯面向物联网领域开发的实时操作系统</font>

TencentOS tiny 是腾讯面向物联网领域开发的实时操作系统，具有低功耗，低资源占用，模块化，安全可靠等特点，可有效提升物联网终端产品开发效率。TencentOS tiny 提供精简的 RTOS 内核，内核组件可裁剪可配置，可快速移植到多种主流 MCU (如 STM32 全系列)及模组芯片上。而且，基于 RTOS 内核提供了丰富的物联网组件，内部集成主流物联网协议栈（如 CoAP/MQTT/TLS/DTLS/LoRaWAN/NB-IoT 等），可助力物联网终端设备及业务快速接入腾讯云物联网平台。

> 项目主页: https://github.com/Tencent/TencentOS-tiny

![](http://henjay724.com/image/biweekly/TencentOS-tiny.PNG)

### <font color="red">3、OneOS - 中国移动针对物联网领域推出的轻量级操作系统</font>

OneOS是中国移动针对物联网领域推出的轻量级操作系统，具有可裁剪、跨平台、低功耗、高安全等特点，支持ARM Cortex-M/R/A、MIPS、RISC-V等主流CPU架构，兼容POSIX、CMSIS等标准接口，支持Micropython语言开发，提供图形化开发工具，能够有效提高开发效率并降低开发成本，帮助客户开发稳定可靠、安全易用的物联网应用。

> 项目主页: https://os.iot.10086.cn/

另外，针对物联网应用的硬件碎片化、网络多样化、接入复杂化以及安全等问题，OneOS 具有如下特性：

![](http://henjay724.com/image/biweekly/OneOS.PNG)

作为一款新晋 RTOS，OneOS 有着精准的行业定位，未来将被广泛运用到智能穿戴、智能门锁、智慧充电、环境监测等智慧系统。

### <font color="red">4、Component Tester - 超迷你的元器件测试仪</font>

Component Tester是印度小伙Akshay Baweja设计的元器件测试仪，前后做了三款不同硬件版本。其实现原理其实很简单，通过ADC将3个管脚上的电压信号量化后再软件处理，核心是支持的那些元器件参数计算方法。

> * 项目主页（钥匙扣型）: https://hackaday.io/project/173267-component-tester-in-a-keychain
> * 项目主页（UNO标准型）: https://hackaday.io/project/175338-component-tester-uno-shield
> * 项目主页（USB接口型）: https://hackaday.io/project/173922-usb-component-tester

这个元器件测试仪支持的器件很多，比如电阻、电容、电感、二极管、晶体管、场效应管、晶闸管、双向可控硅等。下图便是其实测电阻的效果图。

![](http://henjay724.com/image/biweekly/ComponentTester.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


