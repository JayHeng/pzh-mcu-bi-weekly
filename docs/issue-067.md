# 痞子衡嵌入式半月刊： 第 67 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 66 期》](https://www.cnblogs.com/henjay724/p/16863555.html)

## 唠两句

历史上的今天：。

本期共收录 2 个项目、 0 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、TinyMaix - 面向单片机的超轻量级的神经网络推理库</font>

TinyMaix 是专为低资源的单片机设计的 AI 神经网络推理框架，通常被称为 TinyML。TinyMaix 可以让你在任意单片机上运行轻量级深度学习模型。TinyMaix 的设计原则：易用性 > 移植性 > 速度 > 空间。

TinyMaix 其实是矽速科技（Sipeed）利用两个周末的业余时间完成的项目，它足够简单，可以在 30 分钟内读完代码，可以帮助新手理解它是怎么运行的。

> * 项目地址：https://github.com/sipeed/TinyMaix

TinyMaix 关键特性：

```text
- 核心代码少于400行(tm_layers.c+tm_model.c+arch_cpu.h), 代码段(.text)少于3KB
- 低内存消耗，甚至Arduino ATmega328 (32KB Flash, 2KB Ram) 都能基于TinyMaix跑mnist(手写数字识别)
- 支持INT8/FP32/FP16模型，实验性地支持FP8模型，支持keras h5或tflite模型转换
- 支持多种芯片架构的专用指令优化: ARM SIMD/NEON/MVEI，RV32P, RV64V
- 友好的用户接口，只需要load/run模型~
- 支持全静态的内存配置(无需malloc)
- MaixHub 在线模型训练支持
```

### <font color="red">2、ZS1100A - 专用于物联网功耗测量的开源功率计</font>

大多数用于创建物联网(IoT)的设备都是用小电池工作的。由于当前消费电子的动态性，测量这些物联网设备的能耗是一项艰巨的任务。开发人员经常需要使用多种仪器和手工计算来估计能源消耗。ZS1100A 型电能表就是为解决这些问题的。该工具可以非常准确和详细地绘制电流消耗与时间的关系，可以与电池模型一起使用，以估计电池的总体寿命。

> * 项目主页：https://www.crowdsupply.com/zscircuits/zs1100a-power-meter
> * 项目地址：https://github.com/zscircuits/zs1100a

![](http://henjay724.com/image/biweekly20221123/ZS1100A.PNG)

![](http://henjay724.com/image/biweekly20221123/ZS1100A-Spec.PNG)

## 工具类



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

