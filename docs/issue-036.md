# 痞子衡嵌入式半月刊： 第 36 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 35 期》](https://www.cnblogs.com/henjay724/p/15000007.html)

## 唠两句

这周四是大暑，历史上的今天：1991年7月25日，中国长城、故宫、北京人遗址、敦煌莫高窟、秦始皇陵墓五处古迹列为世界遗产。

本期共收录 2个项目、2个工具，希望对你有帮助！

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

