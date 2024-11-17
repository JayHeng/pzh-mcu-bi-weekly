# 痞子衡嵌入式半月刊： 第 111 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 110 期》](https://www.cnblogs.com/henjay724/p/18524019)

## 唠两句

历史上的今天：1843年11月17日，上海开埠，中外贸易中心转移。

本期共 1 个项目、4 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、Zephyr - 面向物联网嵌入式小型可扩展RTOS</font>

Zephyr OS 是一个开源协作项目，旨在为物联网 (IoT) 构建实时操作系统 (RTOS)。它基于专为占用资源的系统而设计的小巧内核，从简单的嵌入式环境传感器和 LED 穿戴式设备到复杂的智能手表和物联网无线网关，应有尽有。

Zephyr 内核具有占用空间较小、高性能、多线程的执行环境及各种可用功能。Zephyr 生态系统的其余部分（包括设备驱动程序、网络堆栈和应用专用代码）使用内核的功能来创建完整的应用。

 * 项目地址：https://www.zephyrproject.org/

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-111/Zephyr.PNG)

## 工具类

### <font color="red">1、CMake - 一个跨平台的自动化构建系统</font>

CMake 是一个跨平台的安装（编译）工具，可以用简单的语句来描述所有平台的安装(编译过程)。它能够输出各种各样的 makefile 或者 project 文件，能测试编译器所支持的 C++ 特性,类似 UNIX下 的automake。只是 CMake 的组态档取名为 CMakeLists.txt。

Cmake 并不直接建构出最终的软件，而是产生标准的建构档（如 Unix 的 Makefile 或 Windows Visual C++ 的 projects/workspaces），然后再依一般的建构方式使用。这使得熟悉某个集成开发环境（IDE）的开发者可以用标准的方式建构他的软件，这种可以使用各平台的原生建构系统的能力是 CMake 和 SCons 等其他类似系统的区别之处。

 * 项目地址：https://cmake.org/

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-111/CMake.PNG)

### <font color="red">2、Ninja - 开源的轻量级快速构建工具</font>

Ninja 是一个小型、快速的依赖驱动的构建系统，由 Google 的 Chris Martine 开发‌。它旨在提高构建速度，通过与其他构建系统（如 CMake 或 Meson）配合使用，生成中间构建文件，从而高效地编译源代码。Ninja 的设计哲学是简化构建过程并优化磁盘和内存的使用，特别适合大规模软件工程的构建‌。

 * 项目地址：https://ninja-build.org/

 ### <font color="red">3、Kconfig - 一种用于配置系统选项和特性的配置系统</font>

Kconfig 是 Linux 内核（以及 Zephyr）一种用于配置系统选项和特性的配置系统。它是一种配置语言和配置工具的组合，用于管理内核的各种功能和选项，使开发者能够根据其需求自定义内核的构建。Kconfig 不仅用于配置内核的构建选项，还用于配置内核中各个功能的开启或关闭状态，从而构建出适合特定硬件和需求的定制化内核。

 * 项目地址：https://github.com/zephyrproject-rtos/zephyr/blob/main/doc/build/kconfig

以下是 Kconfig 的一些关键特点和概念：

```text
- 菜单和选项： Kconfig 使用树形菜单的方式组织各个配置选项。每个菜单都可以包含一系列的配置选项或子菜单，这些选项可以是布尔值、字符串或整数等不同类型的数据。
- 依赖关系： 在 Kconfig 中，配置选项可以有依赖关系。某些选项可能只能在某些条件满足时才能被启用，这些条件可以是其他选项的状态或硬件支持情况。
- 可视化配置界面： Kconfig 提供了一个可视化的配置界面，通常通过 make menuconfig 命令启动。这个界面允许开发者在交互式环境中浏览和配置各种选项，从而生成配置文件。
- 配置文件生成： 配置界面的更改会导致生成一个 .config 文件，其中包含了用户所做的配置选项。这个配置文件可以传递给构建系统，用于指导内核的编译和构建。
- 构建系统集成： Kconfig 集成在 Linux 内核构建系统中，通过 Makefile 和其他构建工具来解析配置选项并根据配置生成适当的编译指令。
```

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-111/Kconfig.PNG)

 ### <font color="red">4、West - 用于Zephyr项目的可扩展命令行管理工具</font>

West 是 Zephyr 项目提供的一款命令行工具，也被 Zephyr 官网称作”瑞士军刀“，可扩展的命令行工具，负责 Zephyr 工作区管理，管理不同的仓库，下载所有 Zephyr 源码以及其他依赖包配置工作区，通过调用其他工具，来实现工程的构建，烧写以及调试，支持添加自定义扩展指令。

 * 项目地址：https://github.com/zephyrproject-rtos/west

### 欢迎订阅325228

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

