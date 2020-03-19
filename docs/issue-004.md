# 痞子衡嵌入式半月刊： 第 4 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 3 期》](https://www.cnblogs.com/henjay724/p/12418233.html)

## 唠两句

今天是惊蛰与春分交节之时，“春分者，阴阳相半也。故昼夜均而寒暑平”。一个“分”字道出了昼夜、寒暑的界限。

新型肺炎在国内已被完全控制住了，可是中国为全世界省下来的宝贵 2 个月，老外根本没珍惜啊，唉...

痞子衡这两周一半时间在公司，另一半还是 work at home，公司预计 4 月中旬才会全面复工。本周跟同事玩了玩投篮比赛，手感不错，赚了红包，在技术群里发给大家同乐了。

本期共收录 2条资讯、3个项目、2个工具、2个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、 格芯推出业界首款基于 22FDX 平台的量产 eMRAM 助力 IoT 及汽车等应用</font>

近日，格芯宣布其基于 22nm FD-SOI (22FDX) 平台的嵌入式、磁阻型非易失性存储器(eMRAM)已投入生产。此次公告表明 eMRAM 可在 IoT、MCU、汽车等低功耗应用中作为先进工艺节点的高性价比选择。

> 格芯官网：https://www.globalfoundries.com

格芯的 eMRAM 产品旨在替代高容量嵌入式 NOR 闪存，帮助设计人员扩展现有的物联网和微控制器单元架构，以实现 28nm 以下技术节点的功率和密度优势。 格芯的 eMRAM 是一款可靠的多功能嵌入式非易失性存储器(eNVM)，已通过了 5 次严格的回流焊实测，在 -40℃ 至 125℃ 温度范围内具有 100,000 次使用寿命和 10 年数据保存期限。FDX eMRAM 解决方案支持 AEC-Q100 2 级设计，且还在开发工艺，预计明年将支持 AEC-Q100 1 级解决方案。 

通过此前的 IEDM 大会的演示中我们可以了解到一些 MRAM 相较于传统嵌入式 NOR 闪存(eFlash)的优点，虽然 MRAM 技术仍然面临一些挑战，但与 eFlash 相比，它的速度更快，功耗更低。

![](http://henjay724.com/image/biweekly/eMRAM-F_VS_eFLASH.png)

由于还未正式面世，具体的技术细节还无法一窥究竟。读者可以从格芯官网的 22FDX 平台介绍上先行了解一下此次格芯推出的eMRAM的相关信息。

### <font color="red">2、意法半导体推出面向智能物联网设备的微控制器 STM32L4+ </font>

意法半导体最新推出的适用于成本敏感且注重功耗的智能物联网设备的微控制器 STM32L4+，主打能源表、工业传感器、医疗传感器、健身跟踪器、智能家居设备等设备，其系列产品的硬件资源如下。

> 芯片主页：https://www.st.com/en/microcontrollers-microprocessors/stm32l4-plus-series.html#overview

![](http://henjay724.com/image/biweekly/STM32L4+.PNG)

STM32L4+ 系列打破了超低功耗芯片中处理能力的限制，内嵌 2MB 的 Flash 和 640KB 的 SRAM，利用 ST 的 2D 硬件图形加速器Chrom-ART Accelerator™ 能够提供更高级的图形操作，从而释放 CPU 的性能；另外在超低功率下，保证了在同类产品中具有最佳的性能。

## 项目类

### <font color="red">1、 murphyzhao/FlexibleButton - 一个基于标准 C 语言的小巧灵活的按键处理库</font>

FlexibleButton 是网友 murphyzhao 维护的一个基于标准 C 语言的小巧灵活的按键处理库，支持单击、连击、短按、长按、自动消抖，可以自由设置组合按键，可用于中断和低功耗场景。

> 项目主页：https://github.com/murphyzhao/FlexibleButton

该按键库解耦了具体的按键硬件结构，理论上支持轻触按键与自锁按键，并可以无限扩展按键数量。另外，FlexibleButton 使用扫描的方式一次性读取所有所有的按键状态，然后通过事件回调机制上报按键事件。核心的按键扫描代码仅有三行，没错，就是经典的 **三行按键扫描算法**。

FlexibleButton 中按键事件的定义并没有使用 Windows 驱动上的定义，主要是方便嵌入式设备中的应用场景，下面是支持的所有按键事件的定义：

```C
typedef enum
{
    FLEX_BTN_PRESS_DOWN = 0,        // 按下事件
    FLEX_BTN_PRESS_CLICK,           // 单击事件
    FLEX_BTN_PRESS_DOUBLE_CLICK,    // 双击事件
    FLEX_BTN_PRESS_REPEAT_CLICK,    // 连击事件
    FLEX_BTN_PRESS_SHORT_START,     // 短按开始事件
    FLEX_BTN_PRESS_SHORT_UP,        // 短按抬起事件
    FLEX_BTN_PRESS_LONG_START,      // 长按开始事件
    FLEX_BTN_PRESS_LONG_UP,         // 长按抬起事件
    FLEX_BTN_PRESS_LONG_HOLD,       // 长按保持事件
    FLEX_BTN_PRESS_LONG_HOLD_UP,    // 长按保持的抬起事件
    FLEX_BTN_PRESS_MAX,
    FLEX_BTN_PRESS_NONE,
} flex_button_event_t;
```

FlexibleButton 使用 C 语言标准库 API 编写，也使得该按键库可以无缝兼容任意的处理器平台，并且支持任意 OS 和 non-OS（裸机编程）。

### <font color="red">2、TinyUSB - 适用于嵌入式系统的开源跨平台 USB 协议栈</font>

TinyUSB 是由网友 hathach 管理维护的一个开源跨平台 USB 协议栈，协议栈中包含了主机端及设备端的协议栈，由于不使用动态内存分配以及采用阻塞所有中断事件，在非 ISR 任务功能中处理中断事件的设计方式，所以此协议栈的内存安全性及线程安全性极高。

> 项目主页：https://github.com/hathach/tinyusb

此协议栈使用信号量/互斥量来访问共享资源，因此需要使用到 OS 的一些 API。目前 TinyUSB 支持 FreeRTOS 及 Mynewt 两种 OS。

![](http://henjay724.com/image/biweekly/TinyUSB_Structure.png)

目前该协议栈支持的 MCU 有：

```text
- MicroChip: SAMD21, SAMD51 (device only)
- Nordic: nRF52840, nRF52833
- Nuvoton: NUC120, NUC121/NUC125, NUC126, NUC505
- NXP: LPC Series: 11Uxx, 13xx, 175x_6x, 177x_8x, 18xx, 40xx, 43xx, 51Uxx, 54xxx, 55xx
       iMX RT Series: RT1011, RT1015, RT1021, RT1052, RT1062, RT1064
- Sony: CXD56
- ST: STM32 series: L0, F0, F1, F2, F3, F4, F7, H7 (device only)
```

如果读者想要在列表以外的 MCU 上使用 TinyUSB，项目主页中有详细的移植过程以供参考。

### <font color="red">3、CPU Stress Detector - 基于 Bolt IoT 无线模组及其云服务的 CPU 负荷检测器</font>

这是来自 Hackaday 上的一个作品，基于 [Bolt IoT](https://www.boltiot.com/) WiFi 模组及其配套云服务和 App 的计算机 CPU 负荷检测器。

> 项目主页：https://www.hackster.io/lahariimmanni2397/cpu-stress-detector-7b8e8b

有时计算机 CPU 会超载发热，CPU 负荷检测器可以检测到这个情况，并通过不同颜色 LED 进行指示。如果 CPU 过载，则红色 LED 点亮并发出警报; 如果 CPU 负荷较低，则绿色 LED 点亮。通过这些指示，我们可以了解 CPU 的压力等级。

![](http://henjay724.com/image/biweekly/CPU-Stress-Detector_circuit.PNG)

PC 端代码采用 Python 编写，直接调用封装好的 [boltiot](https://pypi.org/project/boltiot/) 库来访问 Bolt IoT 云。

```python
import psutil
from boltiot import Bolt

api_key   = "YOUR_API_KEY"
device_id = "YOUR_DEVICE_ID"

cpu_red_threshold = 0.4
client= Bolt(api_key, device_id)

def control_green_led(pin, value):
    response = client.digitalWrite(pin, value)

def control_red_led(pin, value):
    response = client.digitalWrite(pin, value)

while True:
    cpu_usage = psutil.cpu_percent(interval = 5) #检测间隔(s)
    if cpu_usage &gt; cpu_red_threshold:
        control_green_led('0','LOW')
        control_red_led('1', 'HIGH')
        control_red_led('2', 'LOW')
    else:
        control_green_led('0', 'HIGH')
        control_red_led('1', 'LOW')
```

## 工具类

### <font color="red">1、Proteus VSM - 可用于 MCU 在线仿真调试的 EDA 软件</font>

Proteus 是英国 Lab Center Electronics 公司推出的 EDA 软件，VSM 是 Proteus 三大组件之一（另外两个是 PCB Layout、Visual Designer），VSM 主要用于电路和 MCU 仿真调试。

> 工具主页：https://www.labcenter.com/simulation/

笔者读大学时初学单片机便对 Proteus VSM 一见钟情，在手头没有合适的硬件开发板情况下，快速在 Proteus VSM 上搭一个电路，选好 MCU 模型，然后将编译生成的工程 .hex 文件下载进去就可以直接看运行效果了。如果运行结果不对，还可以单步调试程序来解 Bug。

![](http://henjay724.com/image/biweekly/Proteus_VSM_working.gif)

Proteus VSM 目前支持的 MCU 系列非常多，主流 MCU 厂商的产品型号基本都在内，此外 Proteus VSM 也支持所有主流的编译器（IAR/Keil/GCC等）。

![](http://henjay724.com/image/biweekly/Proteus_supported_VSM_family_v2.PNG)

### <font color="red">2、clang-format - 最流行的 C/C++ 代码格式化插件</font>

clang-format，它是基于 Clang 的一个命令行工具，能够自动化格式化 C/C++/Obj-C 代码，支持多种代码风格：Google, Chromium, LLVM, Mozilla, WebKit，也支持自定义风格（通过编写 .clang-format 文件）。

> 工具主页：http://clang.llvm.org/docs/ClangFormat.html

clang-format 的使用特别简单，安装好之后（在 /clang/tools/clang-format/ 路径下），使用如下命令即可将指定源文件格式化：

```shell
# 使用LLVM风格格式化
clang-format -i main.c -style=llvm

# 使用.clang-format自定义风格格式化
clang-format -i main.c -style=.clang-format
```

此外 clang-format 还可以以插件形式集成在 Vim、Emacs、VS Code 等工具中使用。如果你是 Git 用户，clang-format 还提供了脚本用于格式化 patch。

## i.MXRT出品

### <font color="red">1、蛙声科技 - 便携式视频会议拾音器(Nuroum)</font>

Nuroum 诞生于这样一个理念：高品质、易用的会议产品不应该太贵。Nuroum 采用了专利的麦克风阵列(6个)算法，能够智能地拾取室内覆盖范围内经过噪声过滤、回声消除的声音，因此每个人的声音都非常清晰。Nuroum 配备了 3600mAh 的大容量电池，可以连续 30 小时为会议通话供电。

> RT芯片：i.MXRT1021
> 产品主页： https://nuroum.com/
> 官网定价： 99.98 美元起

![](http://henjay724.com/image/biweekly/Nuroum.PNG)

### <font color="red">2、蛙声科技 - 视频会议模块化产品套件(Hamedal)</font>

Hamedal 耳目达，市场定位是，“告别喂喂喂，不用喊的视频会议”，主要针对的场景是企业会议室。套件包括：可以最多支持 5 个集联（Daisy-Chain）的麦克风阵列 SpeakerMic，支持说话人追踪的 AI 摄像头，可以控制会议的触屏。这套产品配备了标准 PC 的 USB 接口，不需要专业人士即可安装。

> RT芯片：i.MXRT1061
> 产品主页： https://hamedal.com/
> 官网定价： 2999 元起

![](http://henjay724.com/image/biweekly/Hamedal.PNG)

