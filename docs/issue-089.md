# 痞子衡嵌入式半月刊： 第 89 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 88 期》](https://www.cnblogs.com/henjay724/p/17924789.html)

## 唠两句

历史上的今天：1982年1月14日，中国成功完成酵母菌丙氨酸转移核糖核酸的人工全合成。

本期共收录 2 个项目、2 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、EmberGL - 为MCU实时2D/3D渲染而设计的开源图形库</font>

EmberGL(Ember Graphics Library) 是一个底层开源图形库，类似于OpenGL/DirectX/Vulkan，专为 MCU 和其他内存受限的非 GPU 系统上的实时 2D/3D 渲染而设计。图形 API 是专门为这样的系统设计的，利用现代技术能够在紧张的内存空间下最大化渲染性能，同时提供了大量的灵活性和可定制性。

EmberGL 库也可以用于内存更充裕的其他目标，并且可以使用 Visual Studio 和 GCC 等进行编译。因为 EmberGL 是一个低级库，它只提供了灵活高效的 triangle rasterization 的核心呈现功能，以及支持组件和一组显示驱动程序。这些底层特性既可以用于直接的应用程序开发，也可以用于高效的高级图形库(如GUI库或3D引擎)的开发。

 * 项目地址：https://github.com/EmberGL-org/EmberGL

下图展示的是一款 MCU 下 DMA 方式驱动 ILI9341 型 LCD 的效果：

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-089/EmberGL.gif)

### <font color="red">2、Mini-Mars-Rover - 为教育平台建造的火星探测器</font>

Mini-Mars-Rover 是作为一个教育平台建造的火星探测器，它可以激发大家学习编程、电子、技术和太空。围绕新的树莓派 Pico W 的构建可以用 MicroPython 编程，并通过用 Python 编写的服务器应用程序通过 WiFi 进行控制。当然，所有的电子设备都可以用 Arduino 来代替。机器人的底盘是用开放式机器人平台建造的，所以很容易设计支架、适配器和零件。

 * 项目地址：https://github.com/NikodemBartnik/Mini-Mars-Rover

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-089/Mini-Mars-Rover.PNG)

## 工具类

### <font color="red">1、SuperCom - 超强日志显示的串口调试工具</font>

SuperCom 是超级串口调试工具，用于 Window 串口日志的采集、存储、可视化等功能。

 * 工具地址：https://github.com/SuperStudio/SuperCom

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-089/SuperCom.PNG)

SuperCom 美观、流畅、功能丰富、高效，支持以下特点：

```text
- 同时打开多个串口进行监听
- 串口日志自动保存
- 串口日志支持滚屏/固定
- 可以设置波特率、位大小等串口设置
- 可发送各种 AT 指令
- 具有各种特性
```

### <font color="red">2、com0com - 开源的虚拟串口软件</font>

com0com 又名 Null-modem emulator，是一款开源的 Windows 系统内核模式虚拟串行端口驱动程序。com0com 允许创建无限数量的虚拟 COM 端口对以及使用任意端口对连接两个基于 COM 端口的应用程序。每个 COM 端口对提供两个 COM 端口，从一个端口向另一个端口的输出对那个端口来说是输入，反之亦然。

com0com 可以用于为设备模拟器提供串行接口。这种情况下设备模拟程序使用端口对的一个端口，另一个端口由需要通过 COM 端口与设备通信的 Windows 或 DOS 应用程序使用。

 * 工具地址：https://com0com.sourceforge.net/

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-089/com0com.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

