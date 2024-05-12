# 痞子衡嵌入式半月刊： 第 100 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 99 期》](https://www.cnblogs.com/henjay724/p/18169163)

## 唠两句

历史上的今天：1951年5月12日，第一颗氢弹爆炸试验成功。

本期共收录 4 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、GT-HMI-Engine - 专为国内嵌入式GUI设计开发打造的免费神器</font>

GT-HMI 是国产开源 GUI 框架及永久免费设计软件。它提供创建具有易于使用的图形元素，精美的视觉效果和低内存占用的嵌入式 GUI 所需的一切。针对国内市场及用户需求，使用习惯进行了优化设计，为国内工程师量身打造！产品由中国高通 GENITOP 倾心打造，继承了中国高通 30 年的汉显技术及汉字技术积累。产品分为上位机 GT-HMI Designer 和下位机 GT-HMI Engine。  

 * 项目地址：https://gitee.com/genitop/GT-HMI-Engine

GT-HMI 特性：

```text
- 上位机设计软件 GT-HMI Designer 永久免费，下位机技术框架 GT-HMI Engine 开源，使用无拘束；
- GT-HMI Designer 内嵌下位机技术框架编译器，可自动生成下位机代码；
- 提供 GT-HMI 模块，已适配 GT-HMI 上下位机软件及驱动，可以用于前期开发调试，也可以直接作为显示模块使用；
- 多平台兼容，移植便捷；
- 上位机设计软件 GT-HMI Designer；
- 可直接生成交互代码，免去写代码的繁琐工作；
- 模拟器仿真即见即所得；
- 内置了大量常用的组件，如按钮、文本框、进度条、单选框等；
- 支持高通全系列点阵/矢量字库，支持中外文及小语种，多种字号及字体；
- 内置中英文及数字输入法；
- 持续更新的 GUI 示例库和 UI 资源库；
- 下位机技术框架 GT-HMI Engine；
- 纯 C 语言编写，使用无门槛；
- 小巧高效，不限平台，最小仅需 24K RAM+32K FLASH，可运行在 Cortex-ARM M0\M3 等小资源平台；
- 移植便捷，切换平台只需移植定时器、TP 和 LCD 接口，并提供移植教程及示例；
- 丰富详实的例程，配套的开发套件易于上手；
- 支持自定义功能开发，可用 GT-HMI Engine 自定义控件和功能，组合进 GT-HMI Designer 生成的标准代码；
- 带系统（如 RTOS、Linux 等）和裸机均可使用。
```

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-100/GT-HMI-Engine.gif)

### <font color="red">2、inav - 基于STM32F411的导航飞行控制器</font>

inav 是一款基于 STM32F411 设计的导航飞行控制器，全开源，给功能非常强大，目前版本已经演进到 V7。

 * 项目地址：https://github.com/iNavFlight/inav

inav 特性：

```text
- 运行在最流行的STM32F4, AT32, STM32F7和STM32H7飞行控制器
- 屏幕显示(OSD) -字符和像素样式
- DJI OSD集成:所有元素，系统消息和警告
- 出色的开箱即用性能
- 保持位置，保持高度，返回家园和航路点任务
- 优秀的固定翼无人机支持:飞机，飞翼
- 黑匣子飞行记录器记录
- 先进陀螺仪滤波
- 完全可配置的混合器，允许运行任何硬件:多旋翼，固定翼，漫游者，船和其他实验设备
- 多种传感器支持:GPS，皮托管，声纳，激光雷达，温度，ESC与BlHeli_32遥测
- 逻辑条件，全局函数和全局变量:你可以用GUI编程INAV
- SmartAudio和IRC Tramp VTX支持
- 遥测:SmartPort, FPort, MAVlink, LTM, CRSF
- 多色RGB LED带支持
- 屏幕显示(OSD) -字符和像素样式
```

### <font color="red">3、betaflight - 多旋翼/固定翼飞行控制器</font>

betaflight 是用于多旋翼飞行器和固定翼飞行器飞行的飞行控制器软件(固件)。这个分叉与Baseflight和Cleanflight的不同之处在于，它专注于飞行性能，领先的功能添加和广泛的目标支持。

 * 项目地址：https://github.com/betaflight/betaflight

betaflight 特性：

```text
- 支持多色RGB LED条(每个LED可以是不同的颜色，使用可变长度WS2811可寻址RGB条-用于方向指示，低电量警告，飞行模式状态，初始化故障排除等)
- DShot(150,300和600)，Multishot, Oneshot(125和42)和Proshot1000电机协议支持
- 黑匣子飞行记录仪记录(如果配备了机载闪存或外置microSD卡)
- 支持使用STM32 F4, G4, F7和H7处理器的目标
- PWM, PPM, SPI和串行(SBus, SumH, SumD，频谱1024/2048,XBus等)RX连接与故障安全检测
- 多种遥测协议(CRSF, FrSky, HoTT smart-port, MSP等)
- RSSI通过ADC -使用ADC读取PWM RSSI信号，用FrSky D4R-II, X8R, X4R-SB和XSR进行测试
- OSD支持和配置，无需第三方OSD软件/固件/通信设备
- OLED显示器-显示信息:电池电压/电流/毫安时，配置文件，速率配置文件，模式，版本，传感器等
- 飞行中手动PID调整和速率调整
- 使用滑块进行PID和滤波器调谐
- 速率配置文件和它们的飞行选择
- 可配置串行端口，用于串行RX，遥测，ESC遥测，MSP, GPS, OSD，声纳等-使用任何端口上的大多数设备，包括softserial
```

### <font color="red">4、OV-Watch - 硬件成本仅80元的开源智能手表</font>

OV-Watch 是一个基于STM32, FreeRTOS, LVGL的功能强大的智能手表设计。软硬件全开源，目前版本是 V2.3。手表的模式分为3个。第一个是正常的运行模式，手表正常运行；第二个是睡眠模式，MCU进入STOP模式，MPU6050仍在记步数；第三个是关机模式，TPS63020直接关闭使能，此时无3V3供电，只有Vbat有供电。  

 * 项目地址：https://github.com/No-Chicken/OV-Watch

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-100/OV-Watch.png)

从 V1.0 到 V2.3 的版本功能演进：

  ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-100/OV-Watch2.png)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

