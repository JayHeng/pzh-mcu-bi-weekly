# 痞子衡嵌入式半月刊： 第 28 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 27 期》](https://www.cnblogs.com/henjay724/p/14531040.html)

## 唠两句



本期共收录 1条资讯、3个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、Dialog推出低功耗蓝牙降噪耳机应用方案</font>

近日Dialog推出了低功耗蓝牙耳机降噪方案，以下示意框图展示了该方案的所需的各种硬件元件，其中彩色部分Dialog均可以提供相关芯片支持。

通过集成的环境噪声消除（ANC），可以极大提升蓝牙音频耳机收听音乐或对话的能力。 该技术消除了接收到的音频中不想要的背景噪声，同时也将传输的音频信号的干扰降到了最低。 集成使延迟，功耗最小化，并使ANC功能与任何操作系统分离。 集成的USB电池充电器消除了对专用组件的需求，从而使设计具有最小的BOM并提供了最高的性能。

> 资讯主页: https://www.dialog-semiconductor.com/interactive-application-diagram/connected-consumer/bluetoothble-ambient-noise-cancellation-anc-headset

![](http://henjay724.com/image/biweekly20210404/Dialog_blue.png)

## 项目类

### <font color="red">1、玲珑GUI - 面向单片机级别低价产品的开源GUI</font>

玲珑GUI是高效的界面开发解决方案。代替串口屏、组态，降低产品成本，产品软硬件自主可控。配套界面开发软件，图形化编辑界面，生成C代码，直接和用户产品代码结合。配套下载升级软件和bootloader，解决产品升级功能和图片下载问题。

> 项目主页: https://gitee.com/gzbkey/LingLongGUI

![](http://henjay724.com/image/biweekly20210404/LinglongGUI.PNG)

### <font color="red">2、audio-spectrum-visualizer-analyzer - 动感音乐节拍频谱显示器</font>

基于Arduino的32分频、动感音乐节拍频谱器支持多种方式的音频输入，配有四块点阵屏，能够实时显示音乐的频谱信息，随着音乐动感的节拍实时跳动显示。该设计制作简单，可玩性强，如果有对音频处理感兴趣的小伙伴可以动手玩一下。

> 项目主页: https://github.com/shajeebtm/Arduino-audio-spectrum-visualizer-analyzer/

频谱显示器主要有以下5个特点：

```text
1、使用易于安装的库 arduinoFFT 和 MD_MAX72xx。
2、支持五种不同的显示模式，可通过按钮切换。
3、音频信号的左右声道都是混合的，不会错过任何节拍。
4、原型使用 32x8 LED 点阵，你可以随意改变。
5、音频可以从耳机输入或播放设备的Line-Out输入。
```

![](http://henjay724.com/image/biweekly20210404/audio_player.JPG)

ATmega328P内置ADC，可以将输入音频信号转换为数字信号。 ADC的 采样时钟频率为 38.46khz ，通过将 ADC 预分频器配置为32分频来实现。采样频率为 38.64Khz意味着数字样本可以高达19.32Kz的输入频率，这就满足奈奎斯特采样定理。ArduinoFFT 库是将输入模拟信号转换为频谱的核心代码。这个库使用简单，支持的点数从16到128。本项目使用的LED 矩阵为32列×8行，通过MD_MAX72xx 库使显示控制部件非常容易。

### <font color="red">3、garden monitor - 基于树莓派的灌溉系统</font>

基于树莓派驱动的物联网滴灌系统利用物联网来监测和维护植物的正常生长，将传感器与植物相结合，实时监测植物状态，配合App软件，可以根据反馈的数据做出对应的操作来保证植物的健康生长。整个系统由树莓派采集数据信息，例如光照、温湿度和土壤中的水分含量等，随后将各种传感器的数据传送到云数据库中进行处理。使用智能手机应用程序在任何地点支持访问，用户在手机APP上将指令（例如水泵的状态）发送至滴灌系统并执行相关的命令。

> 项目主页: https://make.quwj.com/project/130

![](http://henjay724.com/image/biweekly20210404/garden_monitor.png)


### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

