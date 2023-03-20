# 痞子衡嵌入式半月刊： 第 74 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 73 期》](https://www.cnblogs.com/henjay724/p/17208103.html)

## 唠两句

历史上的今天：1990年3月20日，中国自行设计建造的低温核供热反应堆试运行成功。

本期共收录 2 个资讯、3 个项目、1 个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、2023德国嵌入式展会embedded world近日开幕</font>

第二十一届embedded world嵌入式世界展览与会议于3月14-16日在纽伦堡国际博览中心隆重举办。2023年的展会以“Embedded · Responsible · Sustainable”为主题，在为期三天的展出时间里，带所有参会的企业代表探究全球领先的嵌入式系统产业趋势、交流与分享有趣且精彩的实用案例，并在全球数字化升级的今天领略前沿科技为全领域产业带来变化与进步。

> * 资讯来源：https://www.embedded-world.de/en/press/press-releases/2023/embedded-award-winner-2023

与此同时，embedded world中国站首秀！第一届上海国际嵌入式展（embedded world China 2023）也将于今年6月14-16日在上海世博展览馆3号馆举办。

![](http://henjay724.com/image/biweekly20230320/embedded-world2023.PNG)

### <font color="red">2、兆易创新高性能GD32H7系列MCU近期将正式发布</font>

兆易创新的旗舰级高性能GD32H7系列MCU将于近期正式发布，embedded world 2023展会是GD32H7系列官方开发套件的首秀。

> * 资讯来源：[Embedded World 2023沉浸式逛展，看GD32如何打造完善的生态补给 ](https://mp.weixin.qq.com/s?src=11&timestamp=1679321155&ver=4418&signature=cYyAAI48nTwcWdjuoKwIBN*fiXBov7yvrpfo6wnz6r8*VBC4VLqJSMhRRxcddgovWFryrqrgETBs-A8BYnUSjNAy8PiKivyK*PZ4aaTGVYyfGZT-*Ik8BwThTgW1cjpq&new=1)

GD32H7系列以Arm® Cortex®-M7内核提供600MHz的处理能力，内置先进的DSP和FPU。配备1024KB到3840KB Flash和1024KB SRAM，其中包括512KB的紧耦合内存，以实现更佳处理效率。GD32H7集成了液晶显示屏和硬件图形加速器，可显著提升显示质量，同时还添加了数据安全加密功能。适用于数字信号处理、电机控制、电源、储能系统、音频和语音识别，以及边缘计算、AI等诸多创新应用场景。

![](http://henjay724.com/image/biweekly20230320/GD32H7-EVK.jpg)

## 项目类

### <font color="red">1、USB-Cereal - 全开源的Type-C设备测试开发工具</font>

USB-Cereal 是一个功能强大的完全开源的开发工具，可以简化支持USB Type-C设备的测试、开发、调试和制造。使用USB Type-C的扩展功能，这种独特的硬件附件通过启用调试和工厂日志的捕获，提供简单的命令行界面，并促进固件更新，从而节省时间和精力。

> * 项目主页：https://github.com/oxda/usb-cereal

![](http://henjay724.com/image/biweekly20230320/USB-Cereal2.PNG)

![](http://henjay724.com/image/biweekly20230320/USB-Cereal1.PNG)

### <font color="red">2、MCUFont - 适用MCU系统的字体压缩、解压缩和渲染库</font>

MCUFont 是一个用于 MCU 系统的字体压缩、解压缩和渲染库。它允许高质量的反锯齿文本渲染，同时占用足够小的空间以适应典型的闪存。MCUFont 解码器仅1-5KB，16级抗锯齿，纯C，支持ttf和bdf格式。

> * 项目主页：https://github.com/mcufont/mcufont

### <font color="red">3、DDC OLED - 用电脑HDMI接口中的低速I2C驱动OLED屏</font>

微型 OLED 点阵显示器通常有一个i2c控制器，这个作者搞了一个非常有意思的玩法，将一个控制器直接插入HDMI端口，在HDMI线高速差分对之间，有一个非常慢的i2c总线，使用这个i2c总线来控制OLED。驱动成功后，写点脚本展示功能，可以实现电脑内容在OLED上的显示。

> * 项目主页：https://mitxela.com/projects/ddc-oled

![](http://henjay724.com/image/biweekly20230320/DDC-OLED.PNG)

## 工具类

### <font color="red">1、inspectrum - 开源的无线电信号分析软件</font>

Inspectrum是一个分析捕获信号的工具，信号数据主要来自软件定义的无线电接收机。有网友使用它分析儿童无线玩具车信息，效果还不错。

> * 工具主页：https://github.com/miek/inspectrum

![](http://henjay724.com/image/biweekly20230320/inspectrum.jpg)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

