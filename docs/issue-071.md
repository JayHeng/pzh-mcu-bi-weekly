# 痞子衡嵌入式半月刊： 第 71 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 70 期》](https://www.cnblogs.com/henjay724/p/17054178.html)

## 唠两句

历史上的今天：

本期共收录 4 个项目、1 个工具、0 个RT产品，希望对你有帮助！

## 项目类

### <font color="red">1、JxOS - 面向MCU的小型前后台系统</font>

JxOS 是面向 MCU 的小型前后台系统，提供消息、事件等服务，以及软件定时器，低功耗管理，按键，led 等常用功能模块。在此基础上实现了基于 433 的简单无线网络功能。

> * 项目主页：https://gitee.com/jeremyceng/JxOS

JxOS 项目的设计思想是：功能模块与硬件高度解耦，提高代码模块的可复用性；不使用复杂的数据结构和语法以提高不同硬件平台和编译器之间的兼容性，实现工程在不同 MCU 之间的快速移植；提供实用稳定常用的功能模块，实现项目的快速开发；定义标准应用开发框架，减轻应用开发的工作量和难度。

已使用 JxOS 用于开发项目的硬件平台有：N76E003、STM8S103K、PC、KF8TS2716。

![](http://henjay724.com/image/biweekly20230209/JxOS.PNG)

### <font color="red">2、uLisp - 专门设计用于在有限RAM的MCU上运行的Lisp版本</font>

uLisp 是 Lisp 编程语言的一个版本，专门设计用于在具有有限RAM的微控制器上运行，从基于ATmega328  的 Arduino Un o到 Tenensy 4.0/4.1。无论使用什么平台，都可以使用完全相同的 uLisp 程序。

> * 项目主页：http://www.ulisp.com/

因为 uLisp 是一个解释器，你可以输入命令并立即看到效果，而不需要编译和上传你的程序。这使它成为学习编程或设置简单电子设备的理想环境。

![](http://henjay724.com/image/biweekly20230209/uLisp.PNG)

### <font color="red">3、LC-3 VM - 250行C代码实现简单的虚拟机(LC-3计算机)</font>

虚拟机是一个像计算机一样工作的程序。它模拟了 CPU 和其他一些硬件组件，允许它执行算术、读取和写入内存，并与 I/O 设备交互，就像一台物理计算机一样。最重要的是，它可以理解一种机器语言，你可以用它来编程。

LC-3 VM 项目是模拟一台名为 LC-3 的虚构计算机。LC-3 在教授大学生如何用汇编语言编程方面很受欢迎。与 x86 相比，它有一个简化的指令集，但包含了现代 cpu 中使用的所有主要思想。

> * 项目主页：https://github.com/justinmeiners/lc3-vm

![](http://henjay724.com/image/biweekly20230209/LC-3_VM.PNG)

### <font color="red">4、lc3-vm - 125行C代码实现简单的虚拟机(LC-3计算机)</font>

来自东欧的软件工程师 Andrei Ciobanu 写得更精简的 LC-3 版虚拟机，并且专门写了图文并茂的博客记录实现过程和原理。

> * 项目主页：https://github.com/nomemory/lc3-vm

![](http://henjay724.com/image/biweekly20230209/lc3-vm.PNG)

## 工具类

### <font color="red">1、WinMerge - 堪比beyond compare的开源文件/文件夹比较工具</font>

WinMerge 是一个开源的 Windows 下区分和合并工具。WinMerge 可以比较文件夹和文件，以易于理解和处理的可视化文本格式显示差异。WinMerge 对于确定项目版本之间的更改以及合并版本之间的更改非常有用。WinMerge 可以作为外部差分/合并工具使用，也可以作为独立应用程序使用。此外，WinMerge 有许多有用的支持功能，使比较，同步和合并尽可能简单和有用。

> * 工具官网：https://winmerge.org/

![](http://henjay724.com/image/biweekly20230209/WinMerge.PNG)

## i.MXRT出品

### <font color="red">1、</font>

> * RT芯片：
> * 产品主页： 
> * 官网定价： 

![](http://henjay724.com/image/biweekly20230209/.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

