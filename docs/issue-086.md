# 痞子衡嵌入式半月刊： 第 86 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 85 期》](https://www.cnblogs.com/henjay724/p/17826449.html)

## 唠两句

历史上的今天：

本期共收录 1 个资讯，1 个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、Arm Cortex-M52发布，将人工智能引入超小型端点设备</font>

近日 ARM 宣布推出专为人工智能物联网 (AIoT) 应用而设计的 Arm® Cortex®-M52 处理器，Cortex-M52 处理器是支持 Arm Helium 技术中体积最小、面积与成本效益最好的产品，无需独立单元即可提供DSP功能（数字信号处理），有助于节省面积和成本，并提供可扩展的弹性以足各种性能与配置需求。

 * 资讯来源：https://newsroom.arm.com/news/arm-cortex-m52

Cortex-M52 采用与 Cortex-M55、Cortex-M85 相同的 Armv8.1-M架构，并支持Helium 矢量扩展方案（M-Profile Vector Extension，MVE），能够有效提高 ML（机器学习）与 DSP 应用的性能表现。与前代 Cortex-M33 相比，Cortex-M52 的 ML 性能提升 5.6 倍，DSP 性能则提升 2.7 倍。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-086/cortex-m52.PNG)

## 项目类

### <font color="red">1、cpost - C语言程序上下文切换和解耦</font>

cpost 是一个 C 语言编写的，用于 C 语言程序上下文切换和解耦的工具。cpost 包含 cpost 和 cevent 两个工具，cpost 用于 C 语言的上下文切换，cevent 用于程序模块之间的解耦。

 * 项目地址：https://github.com/NevermindZZT/cpost

cpos t借鉴了 Android 的 Handler 机制，在 C 语言环境中，可以通过调用 cpost 接口，将函数抛出到另外的线程(上下文)中运行，对于某些场景，尤其是嵌入式编程无操作系统环境下的中断延迟处理。

cevent 借鉴了 Android 的广播机制，在 C 语言环境中，当程序运行至相应的位置，可以通过 cevent 接口抛出一个事件，其他模块可以通过注册的方式，监听这个事件，当事件发生时，调用注册的函数，能很大程度上实现模块间的解耦。 

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-086/.PNG)



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

