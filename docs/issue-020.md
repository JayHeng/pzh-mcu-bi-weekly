# 痞子衡嵌入式半月刊： 第 20 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 19 期》](https://www.cnblogs.com/henjay724/p/13942592.html)

## 唠两句

今天是小雪。“小雪”是个比喻，反映的是这个节气期间寒流活跃、降水渐增，不是反映这个节气下很小量的雪。

近日，北方好几个城市都开始降雪了，下雪才能让人真正意识到冬季到来了。2020快要接近尾声了，这一年中国半导体业可谓风头强劲，各种初创企业如雨后春笋，据不完全统计，今年新增了近4.8万家芯片企业，大浪淘沙之后到底哪些企业拥有真正硬实力，能活下去实现国家半导体振兴这一艰巨任务，让我们拭目以待！

本期共收录 1条资讯、4个项目、1个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、乐鑫发布全新低成本IoT芯片 ESP32-C3</font>

千呼万唤始出来，乐鑫正式推出全新低成本 IoT 芯片 ESP32-C3，成本对标 ESP8266，可 pin to pin 兼容 ESP8266 模组；继承 ESP32 成熟软件架构，搭载 RISC-V 处理器。

![](http://henjay724.com/image/bi-weekly/ESP32-C3_v3.PNG)

```text
1. 支持 Wi-Fi + Bluetooth LE 5.0
2. 400 KB SRAM + 384 KB ROM
3. 睡眠状态电流低至 5 μA
```

## 项目类

### <font color="red">1、FossaSat-1 - 有史以来发射到太空的最小卫星</font>

马德里的一个非盈利组织Fossa Systems开发的开源卫星项目，于2019年10月推出，是西班牙第一颗微型卫星。FossaSat-1尺寸仅为5x5x5cm，重量仅为250g，是有史以来发射到太空的最小卫星之一。

> 项目地址： https://github.com/FOSSASystems/FOSSASAT-1

![](http://henjay724.com/image/bi-weekly/FossaSat-1.JPG)

FossaSat-1分为3个主要的40x40mm板：电力系统板，传感器分线板，板载计算机和通信。

FossaSat-1使用廉价的LoRa模块为全球提供免费和开源的物联网通信，学生将能够以低于20欧元的价格与卫星进行通信。

### <font color="red">2、DAPLink - ARM官方开源的一款调试烧录器</font>

DAPLink是ARM官方开源的一款调试烧录器，一开始叫CMSIS DAP，后来改名成了DAPLink。DAPLink可以调试Arm Cortex全系列MCU，不挑厂家，相比ST-LINK和J-Link具有原生优势。 官方的维护一直在更新，未来也会扩充更多功能。

> 项目地址： https://github.com/ARMmbed/DAPLink

![](http://henjay724.com/image/bi-weekly/CMSIS-DAP.PNG)

DAPLink 主要包含如下四大功能：

```text
1. Arm-cortex芯片的调试和烧录（HID）
2. 自带虚拟串口，省去usb转串口（CDC）
3. 拖拽式编程，模拟出u盘，hex或者bin拷贝进行完成烧录（MSC）
4. WEBUSB功能（固件要升级到2050）
```

### <font color="red">3、LittlevGL - 开源嵌入式图形用户界面库</font>

LittlevGL是一个免费的开源图形库，提供了创建嵌入式GUI所需的一切，具有易于使用的图形元素、漂亮的视觉效果和低内存占用。

LittlevGL图形库是用C语言编写的，可以运行在任何嵌入式系统上：STM, NXP，微芯片，飞思卡尔等品牌的微控制器，ARM Cortex-M，-A，intel，AMD或MIPS内核的单片机等等。

> 项目官网： https://littlevgl.cn/ 或 https://lvgl.io/

![](http://henjay724.com/image/bi-weekly/LittlevGL.PNG)

LittlevGL 特点如下：

```text
1. 强大的构建模组  按钮、图表、列表、滑块、图像等
2. 先进的图形  动画、反锯齿、半透明、平滑滚动
3. 多样的输入设备 触摸板、鼠标、键盘、编码器等
4. 多显示器支持 支持同时使用多个TFT或单色显示器
5. 多语言支持  UTF-8格式文字编码
6. 完全自定义  图形元素
```

### <font color="red">4、PlatformIO - 开源的物联网开发生态系统</font>

PlatformIO 是开源的物联网开发生态系统。提供跨平台的代码构建器、集成开发环境（IDE），兼容 Arduino 和 MBED。PlatformIO 使用纯 Python 开发，无需依赖其他第三方库。可以让你在 PC 上创建信用卡般大小的计算机，例如Raspberry Pi, BeagleBone, CubieBoard。

> 项目官网： https://platformio.org/

![](http://henjay724.com/image/bi-weekly/PlatformIO.PNG)

PlatformIO 支持超过 200 个的开发板和超过 15 种的开发平台以及 10 种开发框架，所以绝大多数流行的开发板都是包含其中的。PlatformIO 中收集整理上百种开发库，方便开发者轻松使用。PlatformIO 最初以命令行的形态进行开发，现如今它可以完美配合其它的 IDE 进行使用，比如 Eclipse、Visual Studio、Atom等。

## 工具类

### <font color="red">1、fireTools - 野火出品的多功能调试助手上位机</font>

野火电子出品的多功能调试助手，包含串口调试、网络调试、摄像头调试、PID调试，二进制文件编辑等。该上位机工具使用Qt开发，界面相当漂亮，完全改掉大家对嵌入式小工具粗糙颜值的观感。

> 软件下载： https://ebf-products.readthedocs.io/zh_CN/latest/deskapp/ebf_trace_tool.html

![](http://henjay724.com/image/bi-weekly/fireTools.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


