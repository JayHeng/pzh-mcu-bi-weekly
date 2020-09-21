# 痞子衡嵌入式半月刊： 第 16 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 15 期》](https://www.cnblogs.com/henjay724/p/13625381.html)

## 唠两句

今天是秋分。

本期共收录 1条资讯、2个项目、2个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、地平线发布全新一代边缘 AI 芯片旭日3</font>

近日，地平线在深圳召开了主题为“释放·芯效能”的新产品发布会，正式推出了全新一代的AIoT边缘AI芯片平台——地平线旭日3。

> 资讯主页: https://www.horizon.ai/news-detail.html?id=19 

旭日3 集成了地平线最先进的伯努利2.0 架构 AI 引擎( BPU )，可提供 5TOPS 的等效算力。新的 BPU 架构极大提升了对先进 CNN 网络架构的支持效果，以及极大降低了 AI 运算对 DDR 带宽的占用率。辅以地平线 “天工开物” AI 开发平台，极大简化算法开发与部署过程，降低 AI 产品的落地成本。

![](http://henjay724.com/image/biweekly/horizon_xuri3.PNG)

## 项目类

### <font color="red">1、wukong-robot - 简单、灵活、优雅的中文语音对话机器人</font>

wukong-robot项目是由github网友wzpan等开发并维护的一个开源中文语音对话机器人项目，能够让感兴趣的开发者快速打造个性化的智能音箱。

> 项目主页: https://github.com/wzpan/wukong-robot 

该项目的特性有：

```text
- 模块化。功能插件、语音识别、语音合成、对话机器人都做到了高度模块化，第三方插件单独维护，方便继承和开发自己的插件
- 中文支持。集成百度、科大讯飞、阿里、腾讯等多家中文语音识别和语音合成技术，且可以继续扩展
- 对话机器人支持。支持基于 AnyQ 的本地对话机器人，并支持接入图灵机器人、Emotibot 等在线对话机器人
- 全局监听，离线唤醒。支持 Muse 脑机唤醒，及无接触的离线语音指令唤醒
- 灵活可配置。支持定制机器人名字，支持选择语音识别和合成的插件
- 智能家居。支持和 mqtt、HomeAssistant 等智能家居协议联动，支持语音控制智能家电
- 后台配套支持。提供配套后台，可实现远程操控、修改配置和日志查看等功能
- 开放API。可利用后端开放的API，实现更丰富的功能
- 安装简单，支持多种平台
```

![](http://henjay724.com/image/biweekly/wukong-robot.png)

### <font color="red">2、Mini-DSO - 一款低成本简易示波器</font>

这是一个由STC8A8K MCU制成的简单示波器，单片机采用的是STC8A8K64S4A12工作在27MHz，显示屏采用的是0.96的OLED，分辨率为128x64。该示波器项目容易上手，涵盖必要的测量功能。支持正常模式、单模式、自动模式，有触发方式选择，如电平触发，自带保存设置。
Mini-DSO输入为单通道模式，秒/格大小能支持多种：500ms，200ms，100ms，50ms，20ms，10ms，5ms，2ms，1ms，500us，200us，100us，电压采集范围为0到30V，采样率能够做到250kHz@100us/div.

> 项目主页: https://github.com/CreativeLau/Mini-DSO

![](http://henjay724.com/image/biweekly/Mini-DSO.jpg)

下面是Mini-DSO的器件件清单：

```text
TC8A8K64S4A12 MCU x 1
SSD1306 OLED（SPI）x 1
电阻：
1W 10k x 1
1/4W 2k x 2
1/4W 10k x 1
1/4W 5k x 1
电容：
47uF x 1
0.01uF x 1
LED x 1
EC11编码器x 1
拨动开关x 1
2针端子x 1
插座排：
7针 x 1
2针 x 1
3.7V锂离子电池
具有充电管理功能的5V升压器模块
USB-TTL下载器
```

## 工具类

### <font color="red">1、ASCIIFlow - 一款通过 ASCII 编码来绘制图表的在线工具</font>

如果你对 Microsoft Visio 望而却步,对 Diagram.ly 都觉得麻烦, ASCIIFlow 可能是你的菜。ASCIIFlow 是上世纪九十年代黑客们最爱的制作流程图表方式，全文本易传播，Geek 风格的反璞归真。

> 工具主页: http://asciiflow.com/
> 项目主页: https://github.com/lewish/asciiflow2

ASCII的文本流程图显得简洁明了，可以做到插入灵活，能够节省空间，便于移植，可以用于说明程序实现或者服务构架等等。而且这个工具直接点开网页就可以使用，十分方便！

![](http://henjay724.com/image/biweekly/ASCIIFlow.jpg)

### <font color="red">2、Micro-Lab - 一款极好用的嵌入式开发调试神软</font>

Micro-Lab是风媒电子的号主赵工开发的一款嵌入式调试工具，嵌入式开发者在开发调试过程中遇到的所有痛点在MicroLab中都统一得以解决。

> 项目主页: https://gitee.com/fengmeitech/Micro-Lab

![](http://henjay724.com/image/biweekly/Micro-Lab.png)

Micro-Lab包含许多实用，且令人激动的全新功能：

```text
“全新的串口/网络调试服务及关联模块”
“发送历史永久保存及支持别名”
“串口/网络动态指令编程”
“串口/网络虚拟示波器”
“超级计算器”
“ModBus RTU计算器”
“DTU”
“串口-网络分裂器”
“应用影子分身”
“众多开发辅助工具及资料”
“独创的革命性事件驱动型上位机编程神器"
```

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


