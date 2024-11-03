# 痞子衡嵌入式半月刊： 第 110 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 109 期》](https://www.cnblogs.com/henjay724/p/18464218)

## 唠两句

历史上的今天：。

本期共 4 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、embedded-hal - 嵌入式系统通用HAL驱动</font>

embedded-hal 是构建与平台无关的驱动程序生态系统的基础，为使用微控制器中常用的外设（如GPIO， UART， SPI或I2C）提供了接口。它们允许以通用的方式编写驱动程序（用于传感器、显示器、执行器、网络适配器等），因此它们可以在任何具有嵌入式实现的微控制器上工作，而无需修改它们。它是嵌入式 Rust 生态系统的核心部分，确保了整个系统的互操作性。

 * 项目地址：https://github.com/rust-embedded/embedded-hal

### <font color="red">2、Bus Pirate - 开源总线协议转换调试工具</font>

Bus Pirate 是一个开源硬件调试工具，可以将简单的命令转换为常见的总线协议，如 1-Wire， I2C， SPI， UART，几个led 等。向芯片或传感器发送命令并获得响应，而无需编写一行代码。  

 * 项目地址：https://hardware.buspirate.com/

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-110/BusPirate.PNG)

### <font color="red">3、quadrant - 开源多通道手势音频控制</font>

quadrant 是一种基于距离传感器阵列的人机界面。该设备由4个 TOF 传感器组成，专门用于检测用户手在自由空间中的位置、速度和方向。机载信号处理用于识别手势和其他事件，这些值可以映射到软件和硬件合成器中的各种音乐参数。quadrant 具有 USB， CV 和硬件 midi 输出，因此可以将其连接到计算机，模拟合成器或任何其他兼容设备。  

 * 项目地址：https://github.com/chronopoulos/quadrant-firmware

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-110/quadrant.PNG)

### <font color="red">4、generative-ai-for-beginners - 微软出品免费人工智能入门课程</font>

微软该课程总共 12 周 24 课，帮助初学者探索人工智能（AI）的世界！它包括实践课程、测验和实验，对初学者非常友好。  

 * 项目地址：https://github.com/microsoft/generative-ai-for-beginners

课程内容包含：

```text
- 人工智能的不同方法，包括知识表示和推理（GOFAI）的“好旧”符号方法。
- 神经网络和深度学习，它们是现代人工智能的核心。课程将使用两个最流行的框架——TensorFlow和PyTorch中的代码来说明这些重要主题背后的概念。
- 用于处理图像和文本的神经架构。课程将介绍最新的型号，但可能有点缺乏最先进的技术。
- 不太流行的人工智能方法，如遗传算法和多智能体系统。
```

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-110/generative-ai-for-beginners.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

