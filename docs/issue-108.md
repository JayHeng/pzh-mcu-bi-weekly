# 痞子衡嵌入式半月刊： 第 108 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 107 期》](https://www.cnblogs.com/henjay724/p/18403610)

## 唠两句

历史上的今天：1925年10月2日，英国科学家贝尔德制成世界上第一个电视雏型。

本期共 4 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、AimRT - 一个面向现代机器人领域的运行时开发框架</font>

AimRT 是一个面向现代机器人领域的运行时开发框架。 它基于 Modern C++ 开发，轻量且易于部署，在资源管控、异步编程、部署配置等方面具有更现代的设计。AimRT 致力于整合机器人端侧、边缘端、云端等各种部署场景的研发。 它服务于现代基于人工智能和云的机器人应用，提供完善的调试和性能分析工具链，以及良好的可观测性支持。

AimRT 还提供了全面的插件开发接口，具有高度可扩展性。 它与 ROS2、HTTP、Grpc 等传统机器人生态系统或云服务生态系统兼容，并支持对现有系统的逐步升级。

 * 项目地址：https://github.com/AimRT/AimRT

### <font color="red">2、QuarkTS - 用于小型嵌入式应用程序的开源操作系统</font>

QuarkTS 是一个操作系统，它提供了一个现代环境来构建稳定且可预测的事件驱动多任务嵌入式软件。该操作系统建立在一个协作的准静态调度程序之上，其简化的内核使用链链方法和事件队列实现了一个专门的轮询方案，以提供真正的 FIFO 优先级调度。

QuarkTS 是使用符合 MISRA C 2012 和 CERT 编码标准指南的正式和严格的流程开发的，并辅以针对安全关键应用的多个静态分析检查。

 * 项目地址：https://github.com/kmilo17pet/QuarkTS

QuarkTS 有如下特点： 

```text
- 优先协同调度。
- 时间控制(定时任务和软件计时器)
- 任务间通信原语、队列、通知和事件标志。
- 状态机(分层支持)
- 协同例程。
- 命令行接口(CLI)
```

### <font color="red">3、JPL open-source-rover - 一款开源的缩小版6轮火星漫游车</font>

JPL 开源火星车是一个开源的，自己建造的用来探索火星表面的6轮火星车设计的缩小版。“开源漫游者”的设计完全基于消费者的现货(COTS)部件。该项目旨在为那些想要参与机械工程，软件，电子，机器人技术的人提供教学和学习经验，同时也是崎岖地形的优秀研究平台。不需要事先的技能或知识。

 * 项目地址：https://github.com/nasa-jpl/open-source-rover

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-108/open-source-rover.gif)

### <font color="red">4、MagiClick S3 - 一款基于ESP32-S3的机械宏键盘</font>

MagiClick S3 是一个单键键盘，基于 ESP32-S3 设计的，带有彩色屏幕。软件开发默认使用 CircuitPython。也可以使用 MicroPython, Arduino。

 * 项目地址：https://github.com/MakerM0/MagiClick-esp32s3

MagiClick S3 规格包括：

```text
- 0.85英寸彩色屏幕，128x128分辨率
- esp32-s3，它支持WiFi，闪存和足够大的RAM来帮助添加更多的功能脚本
- 整体操作主要以中间的机械轴按钮为主，机身左右两侧一般作为辅助
- 键盘轴采用可插拔设计，您可以自由选择静音轴或其他
- 内置一个小扬声器，听一个声音是如此容易
- 机载6轴运动传感器
- 在机身后部有一个扩展口
- USB Type-C接口
- 底部有一个重置按钮
- 车载彩色led。
```

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-108/MagiClickS3.png)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

