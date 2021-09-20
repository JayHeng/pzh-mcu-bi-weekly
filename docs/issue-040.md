# 痞子衡嵌入式半月刊： 第 40 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 39 期》](https://www.cnblogs.com/henjay724/p/15230876.html)

## 唠两句

这周四是秋分。明天是中秋节，痞子衡祝各位读者阖家欢乐，幸福团圆。

本期共收录 2个资讯、3个项目、1个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、2021全球电子成就奖评选已开启</font>

全球电子成就奖 (World Electronics Achievement Awards) 旨在评选并表彰对推动全球电子产业创新做出杰出贡献的企业和管理者，各类奖项获得提名的企业、管理者及产品均为行业领先者，充分体现了其在业界的领先地位与不凡表现。  

该奖项由 ASPENCORE 全球资深产业分析师组成的评审委员会以及来自亚、美、欧洲的网站用户群共同评选出得奖者，网上投票已于 9 月开启，将持续到 10 月。  

> 投票主页： https://doublesummits.eet-china.com/electronic.html

其中产品奖共有 11 个分类，大家有空可以去看看，可以通过这次评选了解到电子行业都有哪些公司推出了哪些产品。在**年度微控制器/接口**下，有痞子衡一直在支持的恩智浦 i.MXRT1170 系列，还望大家帮忙投个票。  

![](http://henjay724.com/image/biweekly20210920/2021_World_Electronics_Achievement_Awards.PNG)

### <font color="red">2、五菱 MCU 芯片首次公开亮相</font>

9月15日举办的上汽通用五菱“中国五菱，全球新能源普及者”品牌发布会上，五菱芯片首次公开亮相，五菱造芯片并非是以全部自研的形式，而是选择与供应链厂商合作。

从目前来看，此次五菱芯片的国产芯片合作方应该是芯旺微。这颗五菱芯片采用了基于ChipON自主研发的KungFu32内核架构处理KF32A15X系列。据芯旺微官方介绍，该处理器采用3级流水线，16位/32位混合指令集，KF32A15X最高主频为120Mhz，Flash达到512KB。同时，ChipON还自主研发了开发工具，包括集成开发环境、C编译器和仿真器。真正意义上实现了从芯片到工具链的全自主。

![](http://henjay724.com/image/biweekly20210920/WULING-MCU-002.PNG)

## 项目类

### <font color="red">1、pico-debug - RP2040 Raspberry Pi Pico板的虚拟调试器</font>

Raspberry Pi Pico所使用的RP2040实际上是一个双核Cortex-M0+，一般情况下，我们都只会使用其中一个核，而另外一个核就处于啥事不干的休眠状态。网上有大神 majbthrd 琢磨着把其中一个Cortex-M0+拿来做调试器，这便是 Pico-debug。

> 项目主页： https://github.com/majbthrd/pico-debug

Pico-debug 方案特点如下：

```text
1. 它不需要额外的硬件：一根USB线，加你手上已有的Pico就行；
2. 它不需要额外的上位机软件，只要一个额外提供的 uf2 文件就行；
3. 它直接把其中一个Cortex-M0+变成了 CMSIS-DAP 调试器，而且是无需用户额外连SWD线——直接就在内部对另外一个Cortex-M0+进行调试。
4. 它不占用Flash，只占用 0x2003C000 ~ 0x2003FFFF 区间的 16K RAM。考虑到Pico总共有264KB的SRAM，这种安排实际上保留了绝大部分的SRAM（248KB）给用户使用。
```

### <font color="red">2、CBUF - 极优雅的宏实现环形缓冲区</font>

循环缓冲区是嵌入式软件工程师在日常开发过程中的关键组件。今天推荐的这个 CBUF 模块使用宏实现循环缓冲区，虽然很多人不喜欢以这种方式使用宏，但 CBUF 实现已被证明是快速、高效且工作相对良好的。  

> 项目主页： https://github.com/barraq/BRBrain/blob/master/firmware/CBUF.h

### <font color="red">3、Zoolark - 一款多功能袖珍仪器</font>

全球最著名的众筹网站Kickstarter最近上线了一款叫Zoolark（翻译过来叫梅林雀）的多功能袖珍仪器。主要的定位就是让每个学习电子电路的学生、调试电路的工程师都可以随时、随地便捷地观测信号、调试电路。

> 项目主页： https://www.kickstarter.com/projects/evoinmotion/zoolark-an-engaging-way-to-learn-electronics-and-circuits?ref=discovery&term=zoolark

![](http://henjay724.com/image/biweekly20210920/Zoolark.PNG)

性能指标汇总一下：

```text
1. 信号发生器输出 - 三角波、方波、正弦波，能够从0.1Hz到1MHz可调，幅度8Vpp可调
2. 可编程直流电压源输出 - -4V到+4V可调
3. 直流电源输出 - +5V、-5V（50mA）、+3.3V（200mA）
4. PWM信号输出 - 频率0.1Hz到1MHz可调，占空比10%到90%可调
5. 示波器功能 - 双通道、最高测量到30Vpp/1MHz，采样率为5Msps
6. 频谱分析 - 100Hz - 2.5MHz
7. 电池供电 - 一次充电可以使用1.5小时
```

## i.MXRT出品

### <font color="red">1、科瑞格绿山 - Keurig POP咖啡机</font>

Keurig公司是美国的一家胶囊咖啡及咖啡机生产商，提供家用及商用咖啡机，其主要产品为K-Cup(K杯)。

> * RT芯片：i.MXRT1052   
> * 产品官网： https://www.keurig.com 
> * 官网定价： N/A  

![](http://henjay724.com/image/biweekly20210920/Keurig_POP.jpg)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

