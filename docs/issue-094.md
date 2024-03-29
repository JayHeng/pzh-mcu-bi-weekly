# 痞子衡嵌入式半月刊： 第 94 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 93 期》](https://www.cnblogs.com/henjay724/p/18050235)

## 唠两句

历史上的今天：1876年3月10日，美国发明家贝尔发明电话。

本期共收录 5 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、At-RTOS - 一个用户友好的嵌入式RTOS</font>

At-RTOS 是一个用户友好的嵌入式控制器实时操作系统，专为 ARM Cortex M 系列架构设计。该项目的目标是通过 RTOS 提供许多有用的接口，支持并简化嵌入式固件开发。

 * 项目地址：https://github.com/At-EC/At-RTOS

At-RTOS 的特点：

```text
1. 支持ARM Cortex M系列架构：At-RTOS专为这一特定架构设计，充分发挥其优势，提高嵌入式系统的效率和性能。
2. 实时性：At-RTOS具备良好的实时性能，能够准确响应各类外部事件和任务，保障系统的稳定性和可靠性。
3. 易用性：At-RTOS以用户友好为设计理念，提供简洁清晰的接口和丰富的文档支持，使开发者能够轻松使用和快速上手。
4. 丰富的接口：At-RTOS提供多样化的接口，能够支持各种嵌入式应用的开发需求，包括任务管理、内存管理、通信协议等。
```

### <font color="red">2、microui - 一个极精简且用ANSI C编写的即时模式UI库</font>

Microui 作为一个微小而便携的 ANSI C 立即模式 UI 库，其特点是占用极少的内存空间，适用于任何可以绘制矩形和文本的渲染系统。Microui 仅占用大约 1100 行 ANSI C 代码，非常小巧。

 * 项目地址：https://github.com/rxi/microui

Microui 内置了多种控件，包括窗口、可滚动面板、按钮、滑块、文本框、标签、复选框和自动换行的文本。

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-094/microui.PNG)

### <font color="red">3、Blinker Library - 一套跨硬件、跨平台的物联网解决方案</font>

Blinker Library 是一套跨硬件、跨平台的物联网解决方案，提供 APP 端、设备端、服务器端支持，使用公有云服务进行数据传输存储。可用于智能家居、数据监测等领域，可以帮助用户更好更快地搭建物联网项目。

 * 项目地址：https://github.com/blinker-iot/blinker-library

Blinker Library 的特点：

```text
- 其由服务器端、app端、设备端组成，可以部署到几乎所有物联网平台
- app端支持ios、android
- 设备端可以使用蓝牙、WiFi、MQTT等方式接入，支持Arduino、freeRTOS、mbed OS、Linux等开发平台
- 服务器端可以部署到阿里云、腾讯云、OneNET、百度云、AWS、google cloud等平台
- 通过界面布局器，免费版用户可自己拖拽布局设备控制界面，自由打造您的物联网设备
- 通过专属SDK，专业版用户可以使用Blinker开发自己的产品，并用于商业用途
```

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-094/BlinkerLibrary.PNG)

### <font color="red">4、ESPUI - 一个适用ESP32/8266的web用户界面库</font>

ESPUI 是一个为 ESP32 和 ESP8266 设备设计的简单的网络用户界面库。它使用户能够轻松地创建和管理设备的 Web 界面，无需任何 HTML、CSS 或 JavaScript 前端开发知识。ESPUI 库可以让用户通过网络浏览器轻松地与设备进行通信和控制，为用户提供了方便、直观的操作界面。

 * 项目地址：https://github.com/s00500/ESPUI

ESPUI 的特点：

```text
1. 简单易用：ESPUI提供了简单易懂的API，用户可以轻松地使用这些API创建自己的Web界面，并且无需掌握专业的前端开发知识。
2. 灵活定制：ESPUI库允许用户根据自己的需要对Web界面进行定制，包括样式、布局和功能等方面。
3. 轻量级：ESPUI库的体积较小，运行效率高，可以在资源受限的微控制器上运行。
4. 支持多种控件：ESPUI库提供了丰富的控件库，包括文本框、按钮、滑块等，满足用户对Web界面的各种需求。
```

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-094/ESPUI.PNG)

### <font color="red">5、WLED - 一套适用WS2812B等数字RGB LED的无线控制库</font>

WLED 是一个快速和功能丰富的实现 ESP8266/ESP32 网络服务器来控制 NeoPixel (WS2812B, WS2811, SK6812) led 或基于 SPI 的芯片组，如 WS2801和APA102。它提供了丰富的功能和灵活的配置选项，使用户能够轻松地创建独特的照明效果。

 * 项目地址：https://github.com/Aircoookie/WLED

WLED 的特点：

```text
1. 多种LED灯带支持：WLED不仅支持WS2812B，还兼容许多其他类型的数字RGB LED灯带，如APA102、SK6812等。这使得用户可以根据自己的需求选择合适的LED灯带。
2. WiFi控制：WLED通过WiFi连接，可以通过智能手机、平板电脑或电脑等设备进行远程控制。用户只需在设备上安装WLED应用程序或通过Web浏览器访问WLED的Web界面，即可方便地控制LED灯带。
3. 丰富的动画效果：WLED内置了大量的动画效果，如彩虹、呼吸灯、闪烁等，用户可以根据自己的喜好选择合适的动画效果，为房间或场景增添独特的氛围。
4. 定时任务和计划：WLED支持设置定时任务和计划，用户可以根据需要自动调整LED灯带的亮度、颜色和动画效果。例如，可以设置在特定时间自动开启或关闭LED灯带，或者在特定日期播放特定的动画效果。
```

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

