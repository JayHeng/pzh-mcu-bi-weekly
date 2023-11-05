# 痞子衡嵌入式半月刊： 第 84 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 83 期》](https://www.cnblogs.com/henjay724/p/17781257.html)

## 唠两句

历史上的今天：。

本期共收录 5 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、NuttX - 成熟的实时嵌入式操作系统</font>

NuttX 是一个实时操作系统(RTOS)，强调标准遵从性和小占用空间。从8位到64位的微控制器环境可扩展，NuttX的主要管理标准是Posix和ANSI标准。那些来自Unix和其他常见RTOS(如VxWorks)的附加标准api（在Posix和ANSI标准下不可用的功能或者不适合深度嵌入式环境的功能(如fork())）也被采用。

NuttX 从架构和风格与 linux 非常相似，NuttX 与 uCOS、FreeRTOS 这类已经普及的实时操作系统差异巨大。NuttX 驱动和应用开发，从结构、接口、风格上都和 linux 非常相像，但是又加入了 linux 不具备的元素和实时特性。

> * 项目地址：https://github.com/apache/nuttx

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-084/NuttX.PNG)

### <font color="red">2、Gobot - 下一代机器人/物联网框架</font>

Gobot 是一个机器人、无人机和物联网(IoT)的框架，用 Go 编程语言编写，它提供了一种简单而强大的方法来创建同时包含多个不同硬件设备的解决方案。

> * 项目地址：https://github.com/hybridgroup/gobot

Gobot 目前支持多达 35 个平台：

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-084/Gobot.PNG)

### <font color="red">3、Olive.c - 基于C的简单开源图形库</font>

Olive.c 是非常简单的基于C语言的图形库，没有任何依赖关系，Olive.c 将所有内容逐像素地呈现到给定的内存中。Olive.c 库不关心图像的显示，它只会用像素填充内存，如何处理这些像素取决于用户。

> * 项目地址：https://github.com/tsoding/olive.c

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-084/Olive_c.gif)

### <font color="red">4、wifi_camera - 可实时查看WiFi信号强度的传感器方案</font>

wifi_camera 方案利用传感器阵列从附近的 WiFi 网络捕获 RSSI 值，并将收集到的像素数据发送给主机，主机对捕获的数据进行处理和可视化。目标是制造一种传感器，使 WiFi 信号或多或少实时可见。

> * 项目地址：https://github.com/Neumi/wifi_camera

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-084/wifi_camera.PNG)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-084/wifi_camera.gif)

### <font color="red">5、Rodeostat - 用于进行电化学测量的电位器</font>

Rodeostat 是一个开源的电位器，用于进行电化学测量，它是一种非常灵活的仪器，具有多个输出电压和电流测量范围。

```text
电流测量范围:+/- 1,10,100,1000uA
输出电压范围:+/- 1、2、5、10V
```

Rodeostat 固件实现了许多常见的伏安方法，例如，计时伏安法，线性扫描，循环伏安法和恒压伏安法。软件以基于网络的应用程序的形式提供图形用户界面。

> * 项目地址：https://iorodeo.com/products/rodeostat

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-084/Rodeostat1.PNG)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-084/Rodeostat2.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

