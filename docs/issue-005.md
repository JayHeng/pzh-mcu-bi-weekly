# 痞子衡嵌入式半月刊： 第 5 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 4 期》](https://www.cnblogs.com/henjay724/p/12529381.html)

## 唠两句

今天是清明，也是全国哀悼日，为抗击新冠肺炎疫情斗争牺牲的烈士和逝世同胞表示深切哀悼！

本期共收录 2条资讯、3个项目、2个工具、1个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、美敦力公开 PB560 呼吸机完整设计</font>

随着新冠疫情在全球持续扩散，上周以来，全世界都出现了呼吸机抢购大战。近日，美国的医疗器械龙头企业美敦力响应 FDA 的号召，宣布公开分享其旗下 Puritan Bennett 560（PB 560）呼吸机的设计规范，帮助行业参与者快速评估呼吸机制造方案，应对全球内的新冠肺炎疫情。

> 资料主页：Medtronic.com/openventilator

![](http://henjay724.com/image/biweekly/Medtronic_PB560.png)

美敦力开源了 PB560 的所有的资料，包括源代码，原理图、PCB、BOM 清单、3D CAD 图等，呼吸机主控使用的是意法半导体 ST10F276。

### <font color="red">2、赛普拉斯推出第六代 USB-C 控制器 ACG1F</font>

不久前，赛普拉斯半导体推出了第六代 USB-C 控制器 ACG1F。ACG1F 的推出为笔记本电脑和台式机提供了完整的 USB Type-C 控制解决方案，是一种低成本单端口 USB-C 控制器。

> 资讯地址：https://china.cypress.com/news/cypress-introduces-sixth-generation-usb-c-controllers-pcs-and-notebooks

ACG1F 采用 32 位 Arm Cortex -M0 处理器，并搭载 16-KB 的 Flash 和 4KB 的 SRAM，提供 USB-C 编程能力，以下是ACG1F 的硬件架构图：

![](http://henjay724.com/image/biweekly/Cypress_ACG1F.PNG)

新一代的 USB-C 控制器可以为下一代笔记本电脑和台式机提供最高的 BOM 集成，从而实现更小的设计尺寸并降低了 OEM 成本。另外，ACG1F 还可以用于将旧式 Type-A 数据端口转换为 Type-C 数据端口所需的设备中。

## 项目类

### <font color="red">1、Amethyst - 一个仅 6 颗芯片打造的复古家用电脑</font>

Amethyst 是 Matt Sarnoff 开发的一款经典的家用计算机，它有一个集成式的键盘，能够生成声音和图像，使用 Forth 编程语言，有图像和声音指令、调试器和屏幕编辑功能。

> 项目主页：https://github.com/74hc595/Amethyst

这个电脑只需要 6 块芯片（ATmega1284、FT320X、2 个 74HC157 和 2 个 74HC166），键盘直接焊在板子上，同样支持音频和四个串行 I/O 链接，用于外围任务，如游戏控制或存储设备。整体电路如下：

![](http://henjay724.com/image/biweekly/Amethyst_diagram.jpeg)

这台电脑提供了一个命令行界面，用户可以进行各种操作。更有趣的是，电脑还自带了一个游戏。游戏中，玩家扮演机器人「#」，并从一大推字符中寻找「kitten」。

![](http://henjay724.com/image/biweekly/Amethyst_screen.jpeg)

### <font color="red">2、USB Tester - 一个可以轻松监控 USB 设备的电流及电压的测试仪</font>

USB Tester 是一个来自于 Hackaday 上的项目。通常 USB 设备的硬件故障查找可能会比较麻烦，尤其是在需要检查电流或电压的情况下，而该项目设计了一个 USB 电压电流测试仪可以方便的嵌入 USB 设备的连接中而不必剪断连接线进行电压电流的检测。

> 项目地址： https://hackaday.io/project/6595-usb-tester 

![](http://henjay724.com/image/biweekly/USBTester.png)

除了固件上的 OLED 显示屏可以显示当前接入的 USB 设备的电压、电流以及功率信息以外，该项目还设计了一块蓝牙底座，并且设计了一个手机上的 APP 用以记录数据或查看实时数据。

### <font color="red">3、DoubiBot - 一个基于 ESP8266 的手写机器人</font>

DoubiBot 是一个基于 ESP8266 的手写机器人，可以实现手动报时和天气预报等功能，也可以把它当做一款通用机械臂，下面是这款手写机器人的硬件架构。

> 项目地址：https://github.com/david-pzh/DoubiBot

![](http://henjay724.com/image/biweekly/DoubiBot.jpg)

另外，项目还提供了硬件 PCB，原理图，3D 模型等资料进行参考。这个手写机器人也可以自己制作，只需准备好 ESP8266 开发板，舵机，以及螺丝，拉杆等小零件即可手动组装。

## 工具类

### <font color="red">1、 Pigweed - 一组用于嵌入式开发的工具模块的集合</font>

Pigweed 是谷歌开源的一个嵌入式库(或模块)的集合。使用 Pigweed 模块可以在 32 位微控制器( 即嵌入单电路芯片中的小型计算机)上实现更快、更可靠的开发。

> 工具主页：https://pigweed.googlesource.com

![](http://henjay724.com/image/biweekly/Pigweed.gif)

Pigweed 提供的模块可满足嵌入式开发人员的广泛需求。从整个生命周期来看，Pigweed 从设置，到开发，再到代码提交，都能够有效提高嵌入式开发的效率。

目前，Pigweed 已提供了不少模块，后续将会有更多模块被添加进来。需要注意的是，它仍处于早期开发阶段，目前不适合用于生产。

### <font color="red">2、QR-Code - 基于Python的二维码生成工具</font>

普通的二维码都是黑白条纹的形式呈现的，看起来很普通，你有见过炫酷的二维码吗？QR-Code是一款基于python实现的炫酷二维码的生成工具。

> 工具地址：https://github.com/sylnsfar/qrcode

QR-Code支持使用命令行进行操作，指令如下

```text
myqr 	Words
		[-v {1,2,3,...,40}]
		[-l {L,M,Q,H}]
        [-n output-filename]
		[-d output-directory]
		[-p picture_file]
		[-c]
		[-con contrast]
		[-bri brightness]
```

下面是GIF动态二维码的展示，用户可以利用QR-Code来制作风格鲜明的二维码。

![](http://henjay724.com/image/biweekly/qrcode_demo1.gif)

![](http://henjay724.com/image/biweekly/qrcode_demo2.gif)

## i.MXRT出品

### <font color="red">1、联迪商用 - 扫码支付终端(QM50)</font>

QM50 是一款扫码支付终端。外观新颖，简洁时尚。配备 2.4 寸 TFT 液晶显示器，可显示动态二维码，支持顾客主扫交易。内置专业条码扫描模块，支持顾客被扫交易。内置非接触读卡器，还可实现挥卡闪付收款，并支持语音播报功能。产品通过中国银联动态二维码生成设备测试、qPBOC 认证，安全可靠。适用于餐饮、零售等需要二维码支付的场所。

> RT芯片：i.MXRT1050
> 产品主页： http://www.landicorp.com/product3_656.html
> 参考售价： 299 元

![](http://henjay724.com/image/biweekly/LANDI_QM50.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


