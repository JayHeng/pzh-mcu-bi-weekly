# 痞子衡嵌入式半月刊： 第 36 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 35 期》](https://www.cnblogs.com/henjay724/p/15000007.html)

## 唠两句

这周四是大暑，历史上的今天：1991年7月25日，中国长城、故宫、北京人遗址、敦煌莫高窟、秦始皇陵墓五处古迹列为世界遗产。

本期共收录 4个项目、2个工具，希望对你有帮助！

## 项目类

### <font color="red">1、AntOS - 适用 8051 的超轻量级实时操作系统</font>

AntOS 是一款超轻量级实时操作系统，抢占式调度极简内核，专门为小型家电及轻量型物联网终端设计，适合在8051为内核的MCU上运行。

> 项目主页： https://gitee.com/zeweni/ant-os

AntOS 提供层级服务，可以进行任意裁剪。内核层包含两个子系统，提供 AntOS 最基本的功能；服务层对内核层进行封装，提供组件和服务；应用层提供给发者编写业务逻辑，同时提供移植第三方软件包的接口。

![](http://henjay724.com/image/biweekly20210725/AntOS.PNG)

### <font color="red">2、AT Command  - 一种 AT 命令通信解析模块</font>

AT Command 是一种 AT 命令通信解析模块，支持裸机(at_chat)和OS版本(at)。适用于modem、WIFI模块、蓝牙通信。

> 项目主页： https://gitee.com/moluo-tech/AT-Command

其中无OS版本使用链式队列及异步回调方式处理AT命令收发，支持URC处理、自定义命令发送与解析作业。

OS版本使用前需要根据at_util.h规定的操作系统相关的接口进行移植，如提供信号量操作、任务延时等操作。

![](http://henjay724.com/image/biweekly20210725/AT_Command.PNG)

### <font color="red">3、RIL - 适用嵌入式的无线通信模块(GSM/GPRS/CatM1/NB)管理框架</font>

RIL 是一款专门为嵌入式平台开发的无线通信模组(GSM/GPRS/CatM1/NB-Iot)管理软件。它与其它大型框架(例如Android RIL、Wince RIL)不同的是，它被设计成应用于资源受限物联网终端设备（单片机+无线模组的方案），并提供物联网通信所需的基本功能，包含网络注册、连接管理、短信收发及Socket通信。目前已支持EC21、BG96、 HL8518等模组，相关的应用也在持续更新中。

> 项目主页： https://gitee.com/moluo-tech/ril

RIL 基本特性包含：

```text
1. 包含网络注册、连接、短信收发及Socket通信管理等基本功能。
2. 模组驱动使用插件化方式管理，同一个系统中能够挂载适配多个模组，并能够动态选择模组驱动程序。
3. 通过简单的修改就能够适用于不同的RTOS平台。
4. 内置多种情况下的异常处理机制，保证模组稳定运行。
5. 内置常用组件，如带断点续传功能的HTTP文件下载、TFTP传输、MQTT等。
```

![](http://henjay724.com/image/biweekly20210725/RIL.PNG)

### <font color="red">4、weather-ink-screen - 支持汉朔2.9寸墨水屏E029A01的天气预报</font>

weather-ink-screen 是基于 DUCK 的天气墨水屏硬件项目的固件应用设计，默认支持2.9寸墨水屏，代号029A01。固件使用Arduino开发，使用到的库包括GxEPD2、U8g2_for_Adafruit_GFX、NTPClient、ArduinoJson、ESP_EEPROM等。

> 项目主页： https://gitee.com/Lichengjiez/weather-ink-screen

weather-ink-screen 功能包含天气模式、阅读模式、时钟模式、配网模式、自定义图片模式。

![](http://henjay724.com/image/biweekly20210725/weather-ink-screen.PNG)

## 工具类

### <font color="red">1、Copilot - OpenAI与GitHub联合出品的自动代码生成AI</font>

Copilot 是 GitHub 官方和 openAI 联合为程序员们送上的编程神器。Copilot 由 OpenAI Codex 提供支持，可以理解为 GPT-3 的改进版。它由公开源代码和自然语言的训练，因此它可以很好理解编程语言以及人类语言，从而能够把人类语言转化成代码。

> 工具主页： https://copilot.github.com/

Copilot 能够把注释转化成代码，只需描述出你想要执行的命令，Copilot就能自动为你组装代码。

Copilot 适用于多种框架和语言，在Python、JavaScript、TypeScript、Rudy、Go几种语言上的表现格外突出。目前，Copilot作为Visual Studio Code插件，支持在本地或GitHub Codespaces上使用。

![](http://henjay724.com/image/biweekly20210725/Copilot.PNG)

### <font color="red">2、VirtualLCD - 可用于 GUI 移植的 LCD 模拟器</font>

VirtualLCD 是一款 LCD 模拟器，可用于GUI移植，如ucGUI,emWin,MiniGUI等。

> 工具主页： https://gitee.com/kerndev/VirtualLCD

使用 VirtLCD 时，同样需要一个demo（VirtSTM32）工程编写我们的界面设计代码，调试好之后可以很快地移到 STM32 工程上。

![](http://henjay724.com/image/biweekly20210725/VirtualLCD.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

