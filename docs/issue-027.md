# 痞子衡嵌入式半月刊： 第 27 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 26 期》](https://www.cnblogs.com/henjay724/p/14461270.html)

## 唠两句

惊蛰是上周五的事，历史上的今天：1982年3月13日中共中央将计划生育定为一项基本国策。

本期共收录 2条资讯、5个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、NXP i.MX系列连推新品，助力边缘计算</font>

近日，恩智浦半导体宣布其EdgeVerse™产品系列新增了跨界应用处理器，包括i.MX 8ULP、经Microsoft Azure Sphere认证的i.MX 8ULP-CS（云安全）系列和新一代高性能智能应用处理器i.MX 9系列。新增产品包括EdgeLock安全区域带来的新创新，以提高边缘安全性，以及旨在最大限度提高能源效率的Energy Flex架构。

> 产品主页: https://www.nxp.com/products/processors-and-microcontrollers/arm-processors/i-mx-applications-processors:IMX_HOME

恩智浦在提供交钥匙网络安全解决方案方面拥有丰富的经验，并以此为基础推出了EdgeLock™安全区域，这是一款经过预配置的安全子系统，可简化复杂安全技术的实施，并帮助设计人员规避代价高昂的错误。

在初始部署后使边缘设备保持长期安全是一项挑战，这需要不间断的可信管理服务。恩智浦和Microsoft合作，通过i.MX 8ULP-CS（云安全）应用处理器系列中的Azure Sphere芯片到云安全性，将该功能提供给客户。

经Azure Sphere认证的i.MX 8ULP-CS集成了Microsoft Pluton，Microsoft Pluton作为芯片本身内置的受保护信任根在EdgeLock安全区域上启用，在为大量物联网和工业应用实现高安全性设备安全方面至关重要。

在设计节能的边缘系统时，芯片级能源优化变得越来越重要。恩智浦实施创新的Energy Flex架构，致力于在便携式或插入式设备中延长电池寿命并减少能源浪费。

![](http://henjay724.com/image/biweekly20210314/i.MX8ULP.png)

### <font color="red">2、格芯22FDX射频解决方案为下一代毫米波汽车雷达提供了基础</font>

近日，格芯宣布将与博世合作开发和制造下一代汽车雷达技术。

> 资讯主页: https://www.globalfoundries.com/cn/xinwengao/gexinrglobalfoundriesr22fdxshepinjiejuefanganweixiayidaihaomiboqicheleidatigonglejichu

博世选择格芯作为其合作伙伴，并采用格芯22FDX™射频解决方案，开发制造了用于先进驾驶辅助系统（ADAS）应用的毫米波汽车雷达片上系统（SoC）。ADAS应用通过保持车辆行驶在正确车道上、发出碰撞警告、启动紧急制动、辅助泊车等，帮助驾驶员实现安全驾驶。

格芯22FDX射频解决方案有如下特点：

```text
- 更加优化的SOC设计：格芯的40nm和22FDX RF毫米波解决方案支持存储器，DSP，模拟和RF功能的SoC集成，以处理ADAS的复杂性
- 脱颖而出的制造工艺：格芯的高性能SiGe BiCMOS（SiGe HP）解决方案建立在130nm或90nm平台上，由于具有出色的VCO相位噪声，更高的PA输出功率和SiGe HBT效率，可为ADAS RADAR IC提供世界一流的性能
- 更短的研发时间：格芯的AutoPro™服务包为汽车客户提供了广泛的解决方案和制造服务，从而最大程度地减少了认证工作并缩短了上市时间
```

![](http://henjay724.com/image/biweekly20210314/FDX22.png)

## 项目类

### <font color="red">1、IO Watch - 一款Arduino UNO 制造的可编程手表</font>

IO Watch是一款基于 Arduino UNO 的可编程的手表，它的制造门槛相对较高，但同时它也更成熟、实用，外形也很有设计感，非常的漂亮！

这块仅 10mm 厚的手表可以使用数年，采用 CR2032 电池供电，内置 DS3231 时钟（RTC）芯片，提供精确时间以及温度补偿功能。

> 项目主页: https://mblazevic.com/Projects/iowatch/index.html

材料清单如下：

```text
•Arduino Uno × 1
•ATMega328 × 1
•3V 20mm CR2032 纽扣电池 × 1
•0603 RED LED 二极管 × 12
•DS3231 RTC 芯片 × 1
```

![](http://henjay724.com/image/biweekly20210314/IOWatch.PNG)

### <font color="red">2、Bluetooth Visual Speaker - 一个基于ESP32的蓝牙音箱</font>

Bluetooth Visual Speaker是由github网友redchenjs开发的一款基于ESP32的蓝牙可视化音箱。

> 项目主页: https://github.com/redchenjs/bluetooth_visual_speaker_esp32

此项目有如下特点：

```text
- A2DP音频流
- I2S&PDM输入/I2S输出
- VFX输出（音频FFT / Rainbow / Starsky / ...）
- BLE控制界面（OTA固件更新/ VFX远程控制）
- 音频提示（已连接/已断开/睡眠/唤醒）
- 睡眠和唤醒键
```

此类音箱项目在github上由很多，感兴趣的朋友可以根据相关的资料，自己DIY一个蓝牙音箱，会是一种不错的体验。

![](http://henjay724.com/image/biweekly20210314/Visual_Speaker2.png)

### <font color="red">3、TeenyUSB - 一个简易的STM32的USB协议栈</font>

TeenyUSB是github上由网友xtoolbox开发的一个轻量的USB协议栈，目前专用于STM32的MCU。

> 项目主页: https://github.com/xtoolbox/TeenyUSB

该项目目前支持的类有：

```text
- HID Device&Host
- MSC Device&Host
- CDC ACM Device&Host
- CDC RNDIS Device&Host
- Hub 
```

项目目前实现了HID+CDC+MSC的复合设备demo以及虚拟网卡等demo，感兴趣的朋友可以在自己的设备上尝试enable这些demo，并进行进一步开发。

![](http://henjay724.com/image/biweekly20210221/teenyusb.png)

### <font color="red">4、raylib - 一个使你享受视频游戏编程乐趣的库</font>

raylib是一个在github上有6000+star的明星项目，该项目是一个纯粹的编程库，特别适合于原型设计，工具，图形应用，嵌入式系统以及教育领域。

> 项目主页: https://www.raylib.com/

该项目具有以下特点：

```text
- 没有外部依赖关系，所有必需的库都捆绑在raylib中
- 支持多种平台：Windows，Linux，MacOS，RPI，Android，HTML5等！
- 用PascalCase/camelCase表示法的纯C代码（C99）编写
- 使用OpenGL（1.1、2.1、3.3或ES2.0）加速硬件
- 支持多种字体格式（TTF，XNA字体，AngelCode字体）
- 出色的纹理格式支持，包括压缩格式（DXT，ETC，ASTC）
- 全面的3D支持，包括3D形状，模型，广告牌，高度图等
- 支持动画3D模型（骨骼动画）
- 着色器支持，包括模型和后处理着色器。
- 用于向量，矩阵和四元数运算的强大数学模块：raymath
- 具有流支持（WAV，OGG，MP3，FLAC，XM，MOD）的音频加载和播放
- 具有可配置HMD设备参数的VR立体声渲染支持
- 带有+120个代码示例的庞大示例集合
- 绑定到+50种编程语言
```

![](http://henjay724.com/image/biweekly20210314/raylib.png)

### <font color="red">5、Nuklear - 可快速移植使用的跨平台GUI库</font>

这个仍然是github上的高星项目，一个用ANSI C编写的开源GUI工具包。

> 项目主页: https://github.com/Immediate-Mode-UI/Nuklear

它被设计为一个简单的应用程序嵌入式用户界面，没有任何依赖关系、默认呈现后端或操作系统窗口/输入处理，而是提供了一个高度模块化的、基于库的方法，具有简单的输入状态，并绘制描述基本形状作为输出的命令。

它的功能有：

```text
- 图形用户界面工具包
- 单头文件库
- 代码量精简（〜18kLOC）
- 注重便携性，效率和简单性
- 没有依赖项（如果不需要，甚至没有标准库）
- 低内存占用量，如果需要/需要，可以完全控制内存使用量
- UTF-8支持
- 可自定义的库模块（您只能编译和使用所需的库模块）
```

![](http://henjay724.com/image/biweekly20210314/Nuklear.gif)


### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

