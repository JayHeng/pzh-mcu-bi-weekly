# 痞子衡嵌入式半月刊： 第 119 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 118 期》](https://www.cnblogs.com/henjay724/p/18732888)

## 唠两句

断更半年，虽然早已达成当初立下的做满 100 期目标，但是回想起这个项目挺多人关注的，还是继续为大家带来更新吧。

这一年原创技术文章产量也减了不少，原因是痞子衡所在公司正全力推进各种 AI 工具的使用，确实有了这些 AI 工具之后，痞子衡感觉 CSDN、博客园上一般技术博文真没有啥阅读的必要，完全被 AI 回答降维打击了，痞子衡的一些原创文章也完全沦为了 AI 训练语料，因此有所懈怠。不过回头想想如果博文仅是自己笔记，自娱自乐也是乐趣了。  

本期共 3 个项目、0 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、fifofast - 一个为MCU精心设计的FIFO</font>

FIFO 是最常用的数据结构之一，尤其是在 MCU 上用于实时处理数据输入/输出。尽管有无数的实现方式，但没有一种是针对入门级微控制器进行良好优化的。fifofast 是一个经过专门设计，旨在尽可能减少 CPU 时间和 SRAM 的消耗，同时提供比典型实现更多的灵活性和功能。它非常适合缓冲串行数据、ADC 测量结果或不同时间关键功能之间共享的任意数据。

 * 项目地址：https://github.com/nqtronix/fifofast

fifofast 核心功能如下：

```text
通用数据：FIFO 快速支持任何数据类型，甚至自定义的类型定义
静态内存：无需通过动态内存管理增加额外开销
内联支持：加快执行速度，尤其是从中断服务例程（ISR）中执行时
占用内存少：典型的 FIFO 只有 3 字节的管理开销
易于使用：实现了所有典型的 FIFO 函数（并且它们的工作方式符合用户预期）
支持调试：可与 Atmel Studio 7 内置调试器配合使用
文档完善：源代码中大量使用注释
```

### <font color="red">2、pebble - Kickstarter史上最成功的智能手表项目</font>

Pebble 及其继任者 Pebble Time 是 Kickstarter 史上前两大筹资项目。Pebble 累计售出了超过二百万只智能手表，培养了一个蓬勃发展的开发者社区，开发出了超过一万款 Pebble 应用和表盘。  

Pebble 代码库包含了整个操作系统，它提供了所有标准的智能手表功能：通知、媒体控制、健身追踪、以及对自定义应用和表盘的支持，并且可以在小型ARM Cortex-M微控制器上运行。该操作系统基于FreeRTOS构建，包含了多个内存管理、图形和时间管理模块，并且提供了一个广泛的框架。 

 * 项目地址：https://github.com/google/pebble

### <font color="red">3、HydraMeter - 一个有趣的万用表项目</font>

HydraMeter 是一个有趣的万用表项目，其中大部分功能在现有的商业万用表中并不常见（这也是作者最初启动这个项目的主要原因）。

 * 项目地址：https://github.com/jduffy105/HydraMeter_0.4

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-119/HydraMeter.png)

HydraMeter 核心功能如下：

```text
- 内置有独立的 USB 接口。
- 具有高采样率和图形（波形）显示功能的选择。
- 可拆卸式显示屏，或者非蓝牙类型的其他无线连接方式。
- 长续航能力（最低续航时长为 100 小时，最长 300 小时）
- 高效的二极管测试输出电压（至少为 3.6V）
- 同时测量电压和电流并进行功率计算。
- 该设计已考虑到未来的更新和升级需求。
- 保险丝更换起来会非常方便，无需拆卸仪表即可完成。
- 如果使用可充电电池，那么这些电池应能通过 USB 接口进行充电。
- 主要功能的界面设计完全直观。无需菜单或软键来切换交流/直流模式、测量范围、电阻与导通性的切换，或者任何其他相关设置。只需查看仪表上的按钮、开关或指针，就能立即知晓其当前状态。而且，只需不到两秒钟就能对仪表进行任何“核心”功能的配置。
```

## 工具类




### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

