# 痞子衡嵌入式半月刊： 第 118 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 117 期》](https://www.cnblogs.com/henjay724/p/18708118)

## 唠两句

历史上的今天：。

本期共 3 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、IMU_Array - 全开源32路IMU传感器矩阵列</font>

这个项目使用 iCE40 接了 32 路 IMU 传感器。使用 IMU 可以知道自己相对于地球的位置。它们本质上是机械设备，因此并非万无一失。一种引起关注的方法是将多个 MEMS IMU 放在单个 PCB 上，将其连接到 FPGA，然后将它们的数据一起处理，以获得更灵敏的 IMU 或过滤漂移。当前代码没做任何花哨的数据处理，只是读取 32 个 IMU 数据，或者发送所有数据，或者做一个简单的平均（实际上只是累积）并输出结果（它处理 IMU 的 4 个不同旋转）。

 * 项目地址：https://github.com/will127534/IMU_Array

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-118/IMU_Array.png)

### <font color="red">2、USB-Insight-HUB - 硬件开源的USB3.0 HUB</font>

USB Insight Hub 项目通过 USB Type-C 连接器插入 PC，并提供三个 USB 3.0 下行端口，每个端口都有一个 1.3 英寸的屏幕，显示所连接设备的相关信息。该信息包括操作系统枚举名（COMx、TTYx或驱动器号）、电压和电流。USB Insight Hub 还允许控制 D+/D- USB 2 数据线的单独激活和禁用，以强制枚举和控制每个下游设备的电源。主机上运行的一个小应用程序从操作系统中提取 USB 信息，并通过 USB 将其发送到 Hub。

 * 项目地址：https://github.com/Aeriosolutions/USB-Insight-HUB-Hardware

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-118/USB-Insight-HUB.png)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-118/USB-Insight-HUB2.png)

### <font color="red">3、smart-multipurpose-battery-tester - 开源多功能电池测试</font>

这个项目作者曾经开发过电池容量测试仪(Battery Capacity Tester V2.0)，它主要用于放电电池以测量其容量。在这个新版本中，用户可以对电池充电和放电，有效地将设备变成了一个电池充电器。

 * 项目地址：https://hackaday.io/project/201803-smart-multipurpose-battery-tester/details

以下是与 V2.0 相比的主要升级特性：

```text
1. XIAO ESP32单片机：
新版本使用XIAO ESP32而不是Arduino，在增加WiFi功能的同时提供更小的占地面积。这允许远程监控和控制，使用户能够从任何地方跟踪电池测试结果。
2. 集成充电器电路：
与测试前需要外部充电器给电池充满电的2.0版本不同，新版本的特点是集成了充电电路。这允许用户一次充电和测试电池，使过程更加简化和方便。
3. 紧凑的SMD电流检测电阻：
该版本用紧凑的SMD电流检测电阻取代了V2.0中使用的笨重的陶瓷电阻。这不仅节省了空间，还通过减少热量积累提高了效率，使测试仪更紧凑，更容易操作。
4. 车载电池座：
它包括一个直接安装在PCB上的18650电池支架。这种增强消除了通过螺钉端子连接外部电池的需要，这是V2.0型号的情况。现在，用户可以简单地将他们的18650电池插入板载支架进行快速测试。此外，提供了一个JST连接器，用于连接LiPo电池或其他不适合18650支架的电池尺寸，为可测试的电池类型提供更大的灵活性。
```

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-118/smart-multipurpose-battery-tester.png)

## 工具类

### <font color="red">1、emba - 嵌入式设备固件安全分析仪</font>

EMBA 是为渗透测试人员、产品安全团队、开发人员和负责任的产品经理设计的中央固件分析和 SBOM 工具。它支持完整的安全分析过程，从固件提取开始，通过仿真进行静态分析和动态分析，构建 SBOM，最后生成基于 web 的漏洞报告。EMBA 自动发现固件中可能存在的薄弱环节和漏洞。不安全的二进制文件、旧的和过时的软件组件、潜在的易受攻击的脚本或硬编码的密码就是一个例子。EMBA 是一个命令行工具，可以生成易于使用的网络报告以供进一步分析。

EMBA 协助渗透测试人员、产品安全团队和开发人员识别固件映像中的薄弱环节和漏洞。EMBA 提供了尽可能多的关于固件的信息，测试人员可以决定关注的领域，并负责验证和解释结果。

 * 项目地址：https://github.com/e-m-b-a/emba

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-118/emba.png)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

