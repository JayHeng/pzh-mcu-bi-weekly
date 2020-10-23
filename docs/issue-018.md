# 痞子衡嵌入式半月刊： 第 18 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 17 期》](https://www.cnblogs.com/henjay724/p/13783225.html)

## 唠两句

今天是霜降。霜降是秋季的最后一个节气，是秋季到冬季的过渡。俗话讲“霜降杀百草”，霜降过后，植物渐渐失去生机，大地一片萧索。

距离美国总统大选日还有10天了，美国总统选举一直是全世界关注的热点，毕竟超级强国的任何政策都可能会引发全球效应。到底是特朗普还是拜登？让我们拭目以待。

本期共收录 1条资讯、4个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、安谋中国“周易”Z2 AIPU正式发布！</font>

2020年10月13日，安谋中国正式发布周易Z2 AIPU，该新版本延用了周易AIPU架构。

> IP主页: https://www.armchina.com/ZhouYi.html

周易Z2 AIPU 五大特性如下：

```text
1. 单核算力1-4TOPS
2. 支持SoC多核实现
3. 微架构优化，面积相比上一代减少30%，特定神经网络模型相同算力配置下性能提升100%
4. 优化内存子系统 和 高级带宽节省技术 
5. 新版主要面向中高端安防、智能座舱和ADAS、边缘服务器等应用场景
```

安谋中国为“周易”AIPU的客户提供很多工具来帮助他们进行开发，包括仿真器、编译器和调试器等进行数据的采集、分析。在软件框架之上，通过Arm Compute Library或者合作伙伴的编辑异构计算库，支持Arm NN、安卓NN等多种流行接口，以及合作伙伴的自有OS和Runtime的框架，接入安谋中国提供的驱动层之后均可正常工作。“周易”AIPU也支持业界主流的AI规模框架，包括TensorFlow、ONNX等，未来也将支持更多不同的扩展框架。

![](http://henjay724.com/image/biweekly/Zhouyi_Z2_AIPU_toolchain.PNG)

## 项目类

### <font color="red">1、Cmockery - 谷歌出品的C单元测试的轻量级框架</font>

CMockery 是 Google 发布的用于 C 单元测试的一个轻量级的框架。它很小巧，对其他开源包没有依赖，对被测试代码侵入性小。CMockery 的源代码行数不到 3K，阅读一下 will_return 和 mock 的源代码就一目了然了。

> 项目主页: https://github.com/google/cmockery

CMockery 主要特点：

```text
1. 免费且开源，Google 提供技术支持；
2. 轻量级的框架，使测试更加快速简单；
3. 避免使用复杂的编译器特性，对老版本的编译器来讲，兼容性好;
4. 并不强制要求待测代码必须依赖 C99 标准，这一特性对许多嵌入式系统的开发很有用
```

### <font color="red">2、OfflineSWD - 一款超迷你的SWD离线烧写器</font>

这是一个开源的SWD离线烧写器，非常Mini，带OLED屏，使用STM32F103RET6作为主控，基于ST官方CMSIS-DAP项目进行修改，实现可脱机、可去读保护烧写。

> 项目主页: https://github.com/MBronsom/OfflineSWD

![](http://henjay724.com/image/biweekly/OfflineSWD.jpg)

该SWD离线烧写器功能特性如下：

```text
1. 使用8M FLASH，可使用虚拟U盘向FLASH放置HEX文件或BIN文件进行烧写（BIN较快）
2. 可去除目标板的读保护，直接烧写（烧写后可能需要手动重启）
3. 支持手动切换模式，使离线烧写器支持DAP仿真
4. 安装驱动后可支持虚拟USB转TTL
5. 可离线使用串口调试功能（仅支持英文及常用数字符号）
```

### <font color="red">3、LiPow - 一款USB type-C供电的锂电池充电器</font>

这是一个基于STM32G0的带USB type-C电源传输的锂电池充电器项目，使用了带电源传输的USB type-C为锂聚合物电池充电。支持2s-4s packs的充电和平衡，支持高达100W的充电。

> 项目主页: https://github.com/AlexKlimaj/LiPow-Firmware

![](http://henjay724.com/image/biweekly/LiPow.PNG)

### <font color="red">4、mini-violin - 一款ATtiny单片机制作的PCB小提琴</font>

这是一个小提琴设计的开源项目，电路原理图相当简单。ATtiny85控制着两个LED和一个压电蜂鸣器，此外还有一个按钮来切换歌曲，特别有意思的是，小提琴的琴弦被连接到微控制器的模拟输入端，这样就可以通过接触导电材料来演奏小提琴了。

> 项目主页: https://github.com/Alexandra182/mini-violin

![](http://henjay724.com/image/biweekly/mini-violin.jpg)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


