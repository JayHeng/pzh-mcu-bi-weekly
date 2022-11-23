# 痞子衡嵌入式半月刊： 第 67 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 66 期》](https://www.cnblogs.com/henjay724/p/16863555.html)

## 唠两句

历史上的今天：。

本期共收录 4 个项目、 0 个工具，希望对你有帮助！

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

### <font color="red">3、dynamic_loader - 单片机上实现动态加载功能的函数库</font>

dynamic_loader 是一个在单片机（如：STM32）上实现动态加载功能的函数库，与 Windows 中的 dll，Linux 中的 so 类似，可以将代码动态地从其他的存储介质，动态加载到 RAM 中。

程序使用 dl_load_lib 加载相应的库文件到句柄中，加载成功后可使用 dl_get_func，通过函数名获得相应函数指针，在不需要使用时可使用 dl_destroy_lib 对句柄进行释放。

> * 项目地址：https://gitee.com/wzh1845462801/dynamic_loader
> * 详细介绍：https://www.armbbs.cn/forum.php?mod=viewthread&tid=109952

### <font color="red">4、little-bee-B1 - 开源实用的高性能电流和磁场探头</font>

little-bee-B1 是一种基于各向异性磁电阻(AMR)磁传感器的开源磁场和电流探头。它直接感知磁场，并通过电流传感附件测量电流，该附件由放置在导线周围的有间隙的铁氧体环形体组成，在导线中的电流和传感器所受的磁场之间建立固定的关系。

> * 项目地址：https://github.com/westonb/little-bee-B1

特性如下：

```text
- 可调带宽(10mhz和1mhz)
- 可调增益(1倍和4倍)
- SMA输出连接器
- 连接到任何标准1 MΩ阻抗示波器输入
- 单节AA电池供电(续航4小时)
- 自动归零
```

![](http://henjay724.com/image/biweekly20221123/little-bee-B1.PNG)

## 工具类



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

