# 痞子衡嵌入式半月刊： 第 103 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 102 期》](https://www.cnblogs.com/henjay724/p/18266049)

## 唠两句

历史上的今天：2012年7月1日，全球增加一秒，出现7:59:60

本期共 5 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、CherryUSB - 小而美的嵌入式USB主从协议栈</font>

CherryUSB 是一个小而美的、可移植性高的、用于嵌入式系统(带 USB IP)的 USB 主从协议栈。

 * 项目地址：https://github.com/cherry-embedded/CherryUSB

为了方便用户学习 USB 基本知识、枚举、驱动加载、IP 驱动，因此 CherryUSB 代码具备以下优点：

```text
- 代码精简，逻辑简单，无复杂 C 语言语法
- 树状化编程，代码层层递进
- Class 驱动和 porting 驱动模板化、精简化
- API 分类清晰（从机：初始化、注册类、命令回调类、数据收发类；主机：初始化、查找类、数据收发类）
```

为了方便用户使用 USB 接口，考虑到用户学习过 uart 和 dma，因此 CherryUSB 设计的数据收发类接口具备以下优点：

```text
- 等价于使用 uart tx dma/uart rx dma
- 收发长度没有限制，用户不需要关心 USB 分包过程（porting 驱动做分包过程）
```

考虑到 USB 性能问题，尽量达到 USB 硬件理论带宽，因此 CherryUSB 设计的数据收发类接口具备以下优点：

```text
- Porting 驱动直接对接寄存器，无抽象层封装
- Memory zero copy
- IP 如果带 DMA 则使用 DMA 模式（DMA 带硬件分包功能）
- 长度无限制，方便对接硬件 DMA 并且发挥 DMA 的优势
- 分包功能在中断中处理
```

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-103/CherryUSB.PNG)

### <font color="red">2、tslib - 嵌入式中使用最广泛的电阻触摸屏校正算法库</font>

tslib 是嵌入式系统里用得最多的触摸屏校正算法库，其充分利用了矩阵的平移，旋转和缩放等运算。tslib 常用于对电阻触摸屏的功能调试，能够为触摸屏驱动获得的采样提供诸如滤波、去抖、校准等功能，通常作为触摸屏驱动的适配层，为上层的应用提供了一个统一的接口。

 * 项目地址：https://github.com/libts/tslib

### <font color="red">3、cotParam - 基于C语言的轻量级参数管理框架</font>

cotParam 是一个参数管理框架代码，其功能就是统一管理软件中的各类系统数据参数。该参数管理并不涉及数据是如何储存的。因为有些系统数据并不需要储存起来，只需要进行管理而已。

 * 项目地址：https://gitee.com/cot_package/cot_param

cotParam 主要特点有：

```text
1. 采用表驱动方式统一管理所有参数，包括缺省值、最小值和最大值等
2. 采用宏定义快速注册和添加参数进行管理
3. 支持基本类型参数和字符串参数
4. 支持序列化和反序列化，便于保存和读取校验
5. 可通过串口协议或其他协议调用接口修改参数
```

### <font color="red">4、cotMenu - 轻量级多级菜单控制框架程序</font>

cotMenu 是一个降低了耦合性，完全独立的菜单框架，菜单显示风格和显示平台完全由自己根据需求设计，而菜单操作统一由菜单模块处理即可，提高程序的移植性。

 * 项目地址：https://gitee.com/cot_package/cot_menu

cotMenu 主要特点有：

```text
1. 采用链表方式实现多级菜单（通过配置选择采用动态分配或者数组实现）
2. 菜单框架作为独立模块，拒绝和按键模块、显示模块进行耦合
3. 在十分独立的情况下，也保证不受菜单的显示风格和显示平台影响，可自由选择设计显示风格和显示平台
4. 快捷菜单操作等
5. 可以采用表驱动的方式初始化菜单，提高代码的可读性
```

### <font color="red">5、cotLed - 轻量级LED控制模块</font>

cotLed 是一个轻量级的LED控制软件框架，可以十分方便地控制LED的各种状态，甚至多个LED组合控制，如跑马灯等。

 * 项目地址：https://gitee.com/cot_package/cot_led

cotLed 主要特点有：

```text
1. 移植方便，无需修改，只需要初始化提供读取相关IO 状态写入函数即可
2. 丰富的接口实现，
   -- 可以实现单个LED亮灭、翻转、闪烁、呼吸灯、自定义（如多少秒快闪几次等）等多种要求的功能
   -- 可以实现多个LED组合跑马灯、流水灯等功能
   -- 同时支持上述模式的次数设置等
3. 代码量少，且代码注释丰富，风格统一，便于阅读和使用
4. 如果设置某个LED为呼吸灯模式，则需要保证 cotLed_Ctrl调用周期为1毫秒（优先级需要最高，或者定时器调度效果最好）
5. 非阻塞任务，因此裸机和操作系统都适用（操作系统下非线程安全，最好可以使用读写锁，如果没有读写锁则至少使用互斥锁）
```

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

