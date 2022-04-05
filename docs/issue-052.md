# 痞子衡嵌入式半月刊： 第 52 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 51 期》](https://www.cnblogs.com/henjay724/p/16064331.html)

## 唠两句

今天是清明，历史上的今天：1815年4月5日，印度尼西亚坦博拉火山喷发，是人类历史上有记载的最猛烈火山爆发事件。

本期共收录 3个项目、3个工具，希望对你有帮助！

## 项目类

### <font color="red">1、Qfplib - 专为ARM Cortex-M内核设计的浮点库</font>

Qfplib 是 ARM Cortex-M 内核的 IEEE 754 浮点库家族。Qfplib 有三个分支针对不同的内核，并以不同的优化目标编写。

```text
Qfplib-M0-tiny： 针对ARM Cortex-M0，高度优化的代码大小，仅单精度。
Qfplib-M0-full： 针对ARM Cortex-M0，优化了代码大小和速度，单精度和双精度。
Qfplib-M3： 针对ARM Cortex-M3，高度优化的速度，单精度。
```

> * 项目主页：https://www.quinapalus.com/qfplib.html

下表比较了 Qfplib-M3 与其他库的循环计数。 Qfplib-M3 计时结果是显示的参数值范围内的近似平均值，包括3个周期的调用开销。 它们是使用 LPC1763 微控制器从(单周期)RAM执行的：

![](http://henjay724.com/image/biweekly20220404/Qfplib.PNG)

### <font color="red">2、Opus - 高灵活度的开源音频编解码器</font>

Opus 是用 C 语言开发的一个高灵活度的音频编码器，针对 ARM、x86 有特殊优化。Opus 在各方面都有着明显优势，它同时支持语音与音乐的编码，融合了 SILK 编码方法和 CELT 编码方法。SILK 原本被用于 Skype 中，基于语音信号的线性预测分析（LPC），对音乐支持并不好。而 CELT 尽管适用于全带宽音频，但对低比特率语音的编码效率不高，所以两者在 Opus 中形成了互补。

> * 项目主页：https://www.opus-codec.org/

![](http://henjay724.com/image/biweekly20220404/Opus.PNG)

Opus 特点包括：

```text
1. 比特率从 6kb/s 到 510 kb/s
2. 采样率从 8kHz（窄带）到 48kHz（全频段）
3. 帧大小从 2.5ms 到 60ms
4. 支持恒定比特率（CBR）和可变比特率（VBR）
5. 从窄带到全频带的音频带宽
6. 支持语音和音乐
7. 支持单声道和立体声
8. 支持多达255个通道（多流帧）
9. 动态可调比特率，音频带宽和帧大小
10. 良好的稳健性和隐蔽性
11. 浮点和定点实现
```

### <font color="red">3、NumWorks - 一款基于STM32F412设计的图形计算器</font>

在时尚智能手机盛行的时代，传统的图形计算器看起来就像是黑暗时代的遗物。这就是为什么这款被称为NumWorks的计算器采用了极简设计和明亮的显示屏，很有意义。

研发团队一开始使用 STM32F429 Discoververy 开始原型设计。2.4″LCD屏幕和USB调试端口启动了开发，设计师很快意识到他们的最终产品不需要 SDRAM 或集成的 LCD 控制器。因此，他们最终确定主控为 STM32F412VG。

> * 项目主页：https://www.numworks.com/
> * 模拟器主页：https://www.numworks.com/simulator/

![](http://henjay724.com/image/biweekly20220404/NumWorks.PNG)

## 工具类

### <font color="red">1、Tracealyzer - RTOS可视化追踪调试软件</font>

Tracealyzer是 Percepio 公司开发的一款用于RTOS或基于linux的嵌入式软件系统的可视化跟踪工具，对系统运行时的行为提供了前所未有的洞察方法。帮助开发人员加快固件的开发，减少对系统验证和性能优化所需要的时间。

目前Tracealyzer提供了30多种相互关联的运行时行为视图，包括任务调度、中断、任务之间的相互作用，以及从应用程序代码中记录的用户事件。Tracealyzer作为传统调试的补充，提供更高层次的调试视图，非常适合理解典型的实时问题。

> * 工具主页：https://percepio.com/tracealyzer/

Tracealyzer支持的OS包括：

```text
FreeRTOS、Embedded Studio、Keil RTX5、Linux、On Time RTOS-32、ThreadX、µC/OS-III、VxWorks
```

![](http://henjay724.com/image/biweekly20220404/Tracealyzer.PNG)

### <font color="red">2、Virtual Eval - ADI公司ADC产品在线评估工具</font>

Virtual Eval（虚拟评估）是ADI公司推出的一款综合性在线产品评估工具。Virtual Eval采用详细软件模型来模拟器件关键性能特征，而不要求购买硬件。辛苦劳累的工程师可以配置不同的工作条件和器件特性来建立自定义使用案例。配置设置被发送到ADI公司服务器以执行仿真作业。数秒之内，完成后的仿真结果就会以图表和性能指标的形式显示在浏览器窗口中。 

> * 工具主页：http://beta-tools.analog.com/virtualeval/

![](http://henjay724.com/image/biweekly20220404/VirtualEval.PNG)

### <font color="red">3、Mbed Simulator - 在线 Mbed 模拟器</font>

Mbed 为了方便开发，推出了一个仿真器，可以模拟运行效果，加快开发速度。这个功能有点像 proteus，但是 proteus 对 arm 的支持还不好，而 mbed simulator 可以很好的和 mbed 结合起来。

> * 工具主页：https://simulator.mbed.com/

![](http://henjay724.com/image/biweekly20220404/MbedSimulator2.PNG)

注意： Mbed Simulator是 Mbed Labs 的一部分。Mbed 实验室项目展示了由 Mbed 工程师开发的有趣的项目。然而，这些项目并没有得到 Arm 的积极支持，并且可能随时被添加，删除或中断。

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

