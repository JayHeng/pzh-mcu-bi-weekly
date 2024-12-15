# 痞子衡嵌入式半月刊： 第 114 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 113 期》](https://www.cnblogs.com/henjay724/p/18593841)

## 唠两句

历史上的今天：1982年12月15日，首届茅盾文学奖授奖仪式举行。

本期共 1 条资讯、2 个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、意法推出基于800MHz CM55和600 GOPS Neural-ART的STM32N6</font>

STMicro 近日宣布推出基于 800MHz ARM Cortex-M55 和 600 GOPS 的 Neural-ART 加速器的 STM32N6 微控制器系列芯片。STM32N6 是ST 最新、最强大的 STM32 系列芯片，为 MCU 带来 MPU 级的性能。

 * 资讯来源：https://blog.st.com/stm32n6/

STM32N6 是首款采用 Arm Cortex-M55 并提供高达 4.2MB 连续嵌入式 RAM 的 STM32。此外，该芯片还包括 ST 的 NeoChrom GPU 和 H.264 硬件编码器。STM32N6 是首款嵌入ST Neural-ART 加速器™ 的 STM32 MCU ，该加速器是 ST 内部开发的神经处理单元 (NPU)，专为节能的边缘 AI 应用而设计。它主频为 1GHz，提供高达 600 GOPS，可为计算机视觉和音频应用提供实时神经网络推理。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-114/STM32N6.PNG)

## 项目类

### <font color="red">1、LK - 专为小型系统而设计的SMP内核</font>

LK 是一种 smp 内核，专为移植到各种平台和 cpu 体系结构的小型系统而设计。其本质是一种 BootLoader，类似于 u-boot。它和 u-boot 最大的差别在于，LK 使用了多线程，而 u-boot 是一个单线程的流程。

 * 项目地址：https://github.com/littlekernel/lk

LK 高级特性如下：  

```text
- 完全可重入的多线程抢占内核
- 可移植到许多 32 位和 64 位体系结构
- 支持各种嵌入式和大型平台
- 强大的模块化构建系统
- 在构建时可选择大量实用工具组件
```

### <font color="red">2、SKRTOS_sparrow - 极其微小的实时操作系统内核</font>

SKRTOS_sparrow 是一款极小型 RTOS，代码仅有 400 行，可以将它看成是一个 mini 版本的 FreeRTOS 内核。作者写了多篇博客讲解它的原理，并指导读者一步步完成一个实时操作系统。

 * 项目地址：https://github.com/skaiui2/SKRTOS_sparrow

对于调度层，它实现了动态内存管理、阻塞延时、多线程、临界区、优先级、低功耗空闲任务等功能，与 FreeRTOS 内核的调度层相比，它的遗憾是同优先级（时间片）没有实现。在拓展篇，作者又补充了 IPC 机制，实现了消息队列、信号量、互斥锁三种 IPC 机制，这对于 RTOS 来说完全够用了。

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

