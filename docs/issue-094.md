# 痞子衡嵌入式半月刊： 第 94 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 93 期》](https://www.cnblogs.com/henjay724/p/18050235)

## 唠两句

历史上的今天：

本期共收录 3 个项目，希望对你有帮助！

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

### <font color="red">3、ESPUI - 一个适用ESP32/8266的web用户界面库</font>

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

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

