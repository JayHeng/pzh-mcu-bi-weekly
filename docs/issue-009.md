# 痞子衡嵌入式半月刊： 第 9 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 8 期》](https://www.cnblogs.com/henjay724/p/12922169.html)

## 唠两句


本期共收录 3条资讯、x个项目、1个工具、1个RT产品，希望对你有帮助！

## 资讯类

### <font color="red">1、瑞芯微AI芯片加持百度飞桨，携手加速AI应用落地</font>

瑞芯微Rockchip近日宣布，旗下AI芯片RK1808、RK1806适配百度飞桨(PaddlePaddle)开源深度学习平台，充分兼容飞桨轻量化推理引擎Paddle Lite。此次瑞芯微与百度合作，旨在为AI行业赋能更多应用场景，加速AI产品落地进程。

> 资讯主页: https://www.rock-chips.com/a/cn/news/rockchip/2020/0513/1084.html

瑞芯微AI芯片RK1808及RK1806，内置独立NPU神经计算单元，INT8 算力高达3.0TOPs；采用22nm FD-SOI工艺，相同性能下的功耗相比主流28nm工艺产品降低约30%，在算力、性能、功耗等指标上均有优异的表现。经实测，瑞芯微AI芯片在Paddle Lite中运行MobileNet V1耗时仅为6.5 ms，帧率高达153.8 FPS，二者充分兼容并高效稳定运行。

![](http://henjay724.com/image/biweekly/RK18xx_Paddle_Lite.png)

如上图所示的实测結果可以看出，与手机等移动端常用的国内外主流CPU相比，RK18系列NPU在MobileNET_v1的耗时更少，表现出色，由此证明在AI相关领域，如图像分类、目标检测、语音交互上，专用的AI芯片将带来更出色的效果。

### <font color="red">2、ZLG正式发布AWTK v1.4</font>

近日，ZLG开源GUI引擎AWTK v1.4正式发布。相对于v1.3，新版本中完善了许多细节，增加了部分特性、控件以及API等，同时新增对iOS平台，以及Python、Java、C++等语言的支持。 

> 资讯主页: https://www.zlg.cn/index/pub/awtk.html

AWTK v1.4新增特性：

```text
- 无文件系统时支持多主题
- OpenGL ES支持snapshot
- edit和mledit支持自己指定的软键盘名称
- 点击鼠标右键触发EVT_CONTEXT_MENU事件
- 增加awtk_main.inc，用于标准程序的主函数
- 用SDL重新实现PC版本的线程和同步相关函数 
- edit增加input_type为"custom_password"的类型
```

![](http://henjay724.com/image/biweekly/AWTK_v1.4.jpg)

AWTK全称为Toolkit AnyWhere，是ZLG倾心打造的一套基于C语言开发的GUI框架。旨在为用户提供一个功能强大、高效可靠、简单易用、可轻松做出炫酷效果的GUI引擎，支持跨平台同步开发，一次编程，到处编译，跨平台使用。 AWTK还配套了所见即所得的AWTK Designer界面设计工具、经典示例以及入门指南文档等 。

### <font color="red">3、Microchip推出软件开发工具包和神经网络IP，助力低功耗FPGA智能嵌入式视觉解决方案</font>

随着人工智能、机器学习和物联网的兴起，对边缘应用的解决方案提出了更高的需求，例如缩小体积、减少产热、提高计算性能等。近日，Microchip Technology Inc.（美国微芯科技公司）发布的智能嵌入式视觉解决方案，致力于让软件开发人员能够更方便地在PolarFire®现场可编程门阵列（FPGA）内执行算法，进而满足边缘应用对节能型推理功能日益增长的需求。

> 资讯主页: http://www.microchip.com.cn/newcommunity/index.php?m=Article&a=show&id=594

![](http://henjay724.com/image/biweekly/Microchip_PolarFire.PNG)

VectorBlox加速器软件开发工具包（SDK）是Microchip嵌入式解决方案组合的重要新成员。受益于FPGA的高运算能力，优秀的能耗比，FPGA成为了边缘人工智能应用的理想选择。Microchip的VectorBlox加速器SDK可以帮助开发人员在不学习FPGA工具流或者不具备设计经验的前提下，利用Microchip PolarFire FPGA创建灵活的低功耗覆盖神经网络应用。

## 项目类

### <font color="red">1、</font>


## 工具类

### <font color="red">1、SpeedCrunch - 高精度科学计算器</font>

SpeedCrunch是一款开源的高精度科学计算器，具有快速，键盘驱动的用户界面。

> 软件主页: https://github.com/speedcrunch/SpeedCrunch

![](http://henjay724.com/image/biweekly/SpeedCrunch.PNG)

SpeedCrunch内置80多个数学函数，允许用户使用复数，数字基数，单位转换等执行最高50位精度的计算，其自动完成功能可加快工作速度，提升效率。SpeedCrunch还内置公式簿，可方便用户查看和插入常用的公式，例如圆锥体的体积计算公式等。

## i.MXRT出品

### <font color="red">1、鱼跃医疗 - 高流量呼吸湿化治疗仪</font>

这款高流量呼吸湿化治疗仪所支持的经鼻高流量氧疗（HFNC）是一项新型的氧疗方式，已被国内外大量临床研究证实在缺氧改善治疗中有很高的应用价值。HFNC通过柔软的鼻塞导管将最高达75L/min流量的空氧混合气体，经由加温加湿后输送给患者。

> RT芯片：i.MXRT1052
> 产品主页： https://www.yuyue.com.cn/index.php/news/info/795.html
> 参考售价： 未知

![](http://henjay724.com/image/biweekly/yuwell_tool.PNG)


