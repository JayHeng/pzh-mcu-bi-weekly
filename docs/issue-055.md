# 痞子衡嵌入式半月刊： 第 55 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 54 期》](https://www.cnblogs.com/henjay724/p/16219300.html)

## 唠两句

上周六是小满，历史上的今天：1936年5月28日，艾伦·图灵发表《论可计算数及其在判定问题上的应用》，提出图灵机模型。

本期共收录 1个资讯、3个项目、0个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、先楫半导体推出高性价比RISC-V微控制器 - HPM6300</font>

近日先楫半导体宣布正式推出 HPM6300 系列。继去年 11 月发布全球性能最强 RISC–V 微控制器 HPM6700/6400 系列后，先楫半导体再添新力量——集高性能、高实时、低功耗，高性价比于一身的 RISC-V 通用微控制器。 

> * 资讯主页：http://www.hpmicro.com/about/detail.html?id=9b6bb03a-9062-4a03-b252-012814083945

HPM6300 延承了 HPM6700 高性能的特点，在成本，功耗，DSP等各个方面做了进一步的优化，并推出了QFP封装，进一步扩大先楫MCU产品在市场上的覆盖范围。

![](http://henjay724.com/image/biweekly20220528/HPM6300.PNG)

## 项目类

### <font color="red">1、CherryUSB - 小而美的、用于嵌入式系统的USB主从协议栈</font>

CherryUSB 是一个小而美的、可移植性高的、用于嵌入式系统的 USB 主从协议栈。

> * 项目主页：https://github.com/sakumisu/CherryUSB

CherryUSB 特点包括：

```text
1. 比较全面的 class 驱动，并且 class 驱动全部模板化，方便自主添加
2. 协议栈采用链表动态注册的方式，减少内存占用
3. 树状化编程，方便理清 class 驱动与接口、端点的关系，hub、port、class 之间的关系
4. 标准化的 porting 接口
5. 设备协议栈的使用简化到类如 uart 、dma 的使用，主机协议栈的使用简化到文件的使用
6. 协议栈实现代码简短，并且从上往下看完就能理清 usb 枚举过程和 class 加载机制
7. Api 少，并且分为三类：dcd/hcd api、注册 api、命令回调 api
```

![](http://henjay724.com/image/biweekly20220528/CherryUSB.PNG)

### <font color="red">2、Blimpduino-2 - 开源的小飞艇</font>

Bllimpduino 2 是一款成本非常低的开源自主飞艇。它由 Arduino M0 飞艇控制器板和车载 WIFI 和激光传感器组成。两个矢量差动推进器和一个升力推进器。设计简单,但令人兴奋。 

> * 项目主页：https://www.jjrobots.com/blimpduino-2/

![](http://henjay724.com/image/biweekly20220528/Blimpduino-2.PNG)

![](http://henjay724.com/image/biweekly20220528/Blimpduino-2_ctrl.PNG)

### <font color="red">3、miniDDS - 基于STM32F3的精简DDS库</font>

FatFS 作者 ChaN 老师做的一个 miniDDS 库。方案基于 ST 公司的 STM32F303K8T6，该芯片集成了三个12位D-A转换器（高转换率、多通道、1 Msa/sec）。ChaN 老师在方案实现中详细研究了利用 LUT 数据插值提高合成波形精度的方法。 

> * 项目主页：http://elm-chan.org/junk/mdds_ipol/report.html

![](http://henjay724.com/image/biweekly20220528/miniDDS.PNG)

## 工具类

### <font color="red">1、</font>



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

