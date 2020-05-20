# 痞子衡嵌入式半月刊： 第 8 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 7 期》](https://www.cnblogs.com/henjay724/p/12829344.html)

## 唠两句

今天是小满，小满节气意味着进入了大幅降水的雨季。痞子衡身处江南，江南雨水尤其多，一年基本有一半时间在下雨。

近期最大的新闻莫过于美国对华为的禁令升级，只要是厂商将使用了美国的技术或设计的半导体芯片出口给华为，就必须得到美国政府的出口许可证。老美真是急眼了，华为加油吧，除了胜利，别无选择！

本期共收录 3条资讯、3个项目、1个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、传华为与意法半导体将联合设计车机芯片</font>

近日，日经新闻从消息源获悉，华为将与ST Microelectronics（意法半导体）共同开发芯片。除了智能手机，还包括针对汽车领域（例如自动驾驶）芯片，这将有助于华为研发自动驾驶汽车技术。

![](http://henjay724.com/image/biweekly/huawei_st_auto.jpeg)

意法半导体多年来一直向华为提供用于各种设备的传感器，两家公司一直在进行长期合作，不过此前并没有共同开发过汽车领域的高级芯片。

意法半导体是宝马等著名汽车厂商的主要合作者之一，华为与它合作可以在车机系统及自动驾驶技术方面有更深的研究。华为最近迅速推出了hi-car，而且成立了车BU部门。

### <font color="red">2、安森美半导体推出全新系列QCS-AX2用于Wi-Fi 6E应用</font>

近日，专注于高效能电子产品的安森美半导体宣布新的QCS-AX2芯片组系列已开始提供样品，该系列支持基于增强的Wi-Fi 6E标准的6GHz频段。

> 资讯主页: https://www.onsemi.cn/PowerSolutions/newsItem.do?article=4535 

新产品阵容：

```text
- QCS-AX2-A12：三频(6GHz / 5GHz / 2.4GHz)，采用 (AdaptivMIMO) 技术，支持灵活的8x8或4x4架构
- QCS-AX2-T12：三频并行4x4运行，提供高性能、高性价比的路由器方案
- QCS-AX2-T8：三频并行8空间流架构，用于网状网络节点和主流接入点
```

![](http://henjay724.com/image/biweekly/onsemi_QCS-AX2.jpg)

QCS-AX2系列基于集成的基带和射频(RF)架构，支持关键的Wi-Fi 6E特性，如正交频分多址(OFDMA)、先进的多用户多输入多输出(MU-MIMO)，和160MHz通道支持以实现更快的速度，以及SmartScan通道选择支持以最大化频段的使用。 

### <font color="red">3、瑞萨电子发布支持32位Arm Cortex-M微控制器RA产品家族的灵活配置软件包（FSP）重要更新</font>

瑞萨电子近日发布了面向瑞萨32位Arm® Cortex®-M微控制器RA产品家族的灵活配置软件包（FSP）更新 。FSP 1.0版增加了新的安全和连接功能、高级神经网络、机器学习和电机控制功能，以及增强的编译器、调试器与开发环境。其增强的安全和连接功能可帮助开发人员快速创建安全的IoT端点和边缘解决方案，可适用于工业4.0、楼宇自动化、计量、医疗、消费类可穿戴设备及家用电器等应用。 

> 软件主页: [www2.renesas.cn/fsp](https://www2.renesas.cn/cn/zh/products/software-tools/software-os-middleware-driver/software-package/ra-fsp.html?utm_campaign=mcu_ra&utm_source=press_release&utm_medium=press_release&utm_content=fsp) 

该软件包此次更新的特性有：

```text
- 全新的安全与连接功能，支持完整的芯片到云端连接
- 支持所有主要云服务提供商并实现安全连接，包括Amazon Web Services、Microsoft Azure、Google Cloud Platform及任何第三方MQTT代理
- 安全功能包括安全秘钥生成和持久的秘钥加密存储，针对NIST规格的AES、SHA-2、RSA 2048和Brainpool椭圆曲线（ECC）加密的硬件加速
- 基于TLS的安全MQTT连接
- 支持神经网络、机器学习和电机控制
```

![](http://henjay724.com/image/biweekly/renesas_RA_FSP.png)

## 项目类

### <font color="red">1、EasyLogger - 一款超轻量级、高性能的 C/C++ 日志库</font>

EasyLogger 是一款超轻量级(ROM<1.6K, RAM<0.3K)、高性能的 C/C\++ 日志库，非常适合对资源敏感的软件项目，例如： IoT 产品、可穿戴设备、智能家居等等。相比 log4c、zlog 这些知名的 C/C++ 日志库， EasyLogger 的功能更加简单，提供给用户的接口更少，但上手会很快，更多实用功能支持以插件形式进行动态扩展。

> 项目主页: https://github.com/armink/EasyLogger

EasyLogger 主要特性如下：

```text
1. 支持用户自定义输出方式（例如：终端、文件、数据库、串口、485、Flash...）；
2. 日志内容可包含级别、时间戳、线程信息、进程信息等；
3. 日志输出被设计为线程安全的方式，并支持 异步输出 及 缓冲输出 模式；
4. 支持多种操作系统（RT-Thread、UCOS、Linux、Windows...），也支持裸机平台；
5. 日志支持 RAW格式 ，支持 hexdump ；
6. 支持按 标签 、 级别 、 关键词 进行动态过滤；
7. 各级别日志支持不同颜色显示；
8. 扩展性强，支持以插件形式扩展新功能。
```

EasyLogger 运行效果如下：

![](http://henjay724.com/image/biweekly/EasyLogger_Demo.gif)

### <font color="red">2、pandora_zhongtian_car - 基于RT-Thread的潘多拉智能遥控小车</font>

今天介绍的是基于Rt-Thread的潘多拉麦克纳娒智能车，整体由底盘，驱动，电池，蓝牙，APP控制，全向轮等组成。

> 项目主页: https://github.com/sundm75/pandora_zhongtian_car

智能车主控使用的是潘多拉IoT Board物联网开发板，软件使用RT-Thread-v3.1.3。目前第一阶段遥控功能已经完成，未来还可以继续增加手柄遥控，远程控制、声音控制等功能。

![](http://henjay724.com/image/biweekly/rtt_bluetooth_car.gif)

### <font color="red">3、RT1052-AutoQuad - 基于i.MXRT1052的开源AutoQuad飞控</font>

这是网友jiezhi320参加RT-Thread应用作品征集赛的原创作品，2015年的时候jiezhi320便基于stm32f405rgt6做了一版硬件，但由于UKF算法对CPU占用率太高，2019年的时候作者将其迁移到imx-rt1052上，以期留出足够的资源给大家来给模友们深入开发。

> 作者主页: https://github.com/jiezhi320

硬件板子基于野火1052 mini开发板，传感器是从马家买的现成模块，采用飞线的形式固定在开发板上（后期会重新设计一款小的适合飞控的板子）

![](http://henjay724.com/image/biweekly/RT1052_AutoQuad_View.png)

各个传感器接到IMX-RT1052的SPI3上，进行分时操作。用于控制ESC的PWM信号，使用主控上PWM1和PWM2中的AB通道。GPS模块是一个独立的单元，通过串口接到主控的串口5上。

![](http://henjay724.com/image/biweekly/RT1052_AutoQuad_BlockDiagram.png)

## 工具类

### <font color="red">1、LabVIEW大众版 - 让工程爱好者居家也可以进行创新开发</font>

美国国家仪器（NI）宣布，推出免费下载的针对非商业用户使用的LabVIEW大众版和LabVIEW NXG大众版。而且，该版本提供了与LabVIEW专业版相同的功能。

> 软件主页: https://www.ni.com/zh-cn/shop/labview/select-edition/labview-community-edition.html

![](http://henjay724.com/image/biweekly/LabVIEW_Community.PNG)

LabVIEW大众版包含：

```text
1. LabVIEW 2020大众版和LabVIEW NXG大众版
2. LabVIEW专业版的所有功能
3. 针对Raspberry Pi、BeagleBoard和Arduino平台的LINX工具包
4. 可访问LabVIEW NXG Web模块，以创建基于Web的应用程序
```

LabVIEW大众版和LabVIEW NXG大众版将会让越来越多的制造商和工程师认识这种直观的图形化语言，这些版本无疑将充分调动开发人员的主动性和创造力以及促进新的合作方式。
