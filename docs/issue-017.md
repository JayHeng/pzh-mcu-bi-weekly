# 痞子衡嵌入式半月刊： 第 17 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 16 期》](https://www.cnblogs.com/henjay724/p/13712975.html)

## 唠两句

今天是寒露。寒露是一个反映气候变化特征的节气，是凉爽向寒冷的转折。

本期共收录 3个项目，希望对你有帮助！

## 项目类

### <font color="red">1、znFAT - 国产嵌入式FAT32文件系统解决方案</font>

znFAT是大神于振南维护的一套高效、完备、精简且具有高可移植性的嵌入式FAT32文件系统解决方案。

> 项目主页: https://gitee.com/dbembed/znfat 

该项目的特性有：

```text
- 与FAT32文件系统高度兼容，提供丰富文件操作函数，可实现文件与目录创建、打开、删除，数据的读取与写入等功能。
- 可方便地移植到多种嵌入式CPU平台上，如51、STM32、AVR、PIC、ColdFile、MSP430等。
- 占用RAM与ROM资源极少，并可由使用者视目标平台资源情况进行灵活配置，最小配置情况下，RAM的使用量约在800~900字节，最大配置下约为1300字节。
- 内建独特数据读写加速算法，以及多种工作模式，均可由用户自行配置，以满足不同的速度与功能需求。
- 创新性提出数据写入的实时工作模式，可保证写入到磁盘文件中的数据安全。防止因恶劣工作环境、干扰或其它原因引起的目标平台不可预见的死机或故障，造成数据丢失（实时模式数据写入速度不高，数据直接写入物理扇区，而不在RAM中暂存，并对文件数据进行实时维护）。
- 底层提供简单的单扇区读写驱动接口以及可选的硬件多扇区读、写、擦除驱动接口。（在提供硬件多扇区读、写、擦除驱动的情况下，磁盘格式化与数据读写速度将有近2~4倍的提升，甚至更高。）
- 提供清晰而强大的功能模块裁剪功能，可极大程度减小最终生成的可执行文件的体积，节省ROM资源。
- 提供数据读取重定向功能，使读到的数据无需缓冲暂存，直接流向应用目的。
```

znFAT作者还为该项目专门写了一本书：

![](http://henjay724.com/image/biweekly/znFAT_book.PNG)

### <font color="red">2、NorthFrame - 一个单片机极简图形化状态机框架</font>

NorthFrame是基于非UML极简理念的状态机框架，配合NF_FsmDesigner图形化开发工具，可无负担替代传统switch-case状态机开发。

> 项目主页: https://gitee.com/PISCES_X/NorthFrame 

NorthFrame包含三个组件：

```text
NF_FSM : 极简非UML状态机框架
NF_FsmDesigner : 基于C# Winform开发的状态机图形化开发工具，可直接生成C代码
NF_Signal : 用于代替全局变量的动态信号机制
```

![](http://henjay724.com/image/biweekly/NorthFrame.PNG)

创建一个在VS2012环境中运行的判断QE组合键的状态机例程仅需如下三步：

```text
Step1 : 使用NF_FsmDesigner工具设计绘制状态转换图，并保存为XML文件
Step2 : 点击生成代码，生成C语言代码
Step3 : 在main.c文件中实现按键处理，并发送事件给状态机
```

### <font color="red">3、MonoGUI - 一个黑白图形用户接口系统</font>

MonoGUI是针对电子词典、高级计算器、电子手表、标签打印机、收款机、电子货签等 具有黑白屏幕的小电子设备开发的专用GUI系统。本系统具有结构简单、使用容易、内 存占用小、单线程、处理器负担轻等特点。虽然图形能力仅有黑与白，但其支持完整的 中文显示处理功能（GB18030中2字节汉字，即旧GB13000标准），其Edit控件和中文输 入法（包括九键输入法）功能上达到Windows和Android的输入法水平，且扩展容易。

> 项目主页: https://gitee.com/liuxinouc/MonoGUI 

MonoGUI使用纯C++编写，不依赖于第三方源码，便于移植和调试。配套的工具软件， 如图片转换器、对话框模板编辑器等，全部开源。设计资料完整，文档充实，也是一份 不可多得的研究资料。

![](http://henjay724.com/image/biweekly/MonoGUI.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


