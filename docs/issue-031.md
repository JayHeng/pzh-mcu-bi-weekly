# 痞子衡嵌入式半月刊： 第 31 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 30 期》](https://www.cnblogs.com/henjay724/p/14702657.html)

## 唠两句

上周三是立夏，历史上的今天：1940年5月16日，在枣宜会战中中华民国军事将领张自忠于宜城阵亡，被追授为上将，成为二战中盟军阵亡的最高军衔的将领。

本期共收录 4个项目，2个工具，希望对你有帮助！

## 项目类

### <font color="red">1、CuTest - 最简洁的C语言单元测试框架</font>

CuTest是一款微小的C语言单元测试框，是我迄今为止见到的最简洁的测试框架之一，只有2个文件，CuTest.c和CuTest.h，全部代码加起来不到一千行。麻雀虽小，五脏俱全，测试的构建、测试的管理、测试语句，都全部包含在内。

> 项目主页: http://cutest.sourceforge.net/

### <font color="red">2、LuatOS - 支持lua语言开发的物联网RTOS</font>

合宙LuatOS是运行在嵌入式硬件的实时操作系统，用户编写lua代码就可完成各种功能，只占用很少的内存和Flash空间。

> 项目主页: https://gitee.com/openLuat/LuatOS

![](http://henjay724.com/image/biweekly20210516/LuatOS.PNG)

特点包括：

```text
- 基于Lua 5.3.x
- 低内存需求, 最低32kb, 96kb flash空间
- 硬件抽象层兼容M3/arm/risc-v/win32等
- 可测试,可模拟(qemu)
- 在线升级
- 可裁剪,可扩展
```

### <font color="red">3、EFSM - 一个基于事件驱动的有限状态机</font>

EFSM(event finite state machine，事件驱动型有限状态机)，是一个基于事件驱动的有限状态机，主要应用于嵌入式设备的软件系统中。

> 项目主页: https://gitee.com/simpost/EFSM

EFSM的设计原则是：简单！EFSM的使用者只需要关心：

```text
- 当事件到来时，通过EFSM取得对应事件的处理方法；
- 当特定事件到来，或者条件满足时，调用状态切换方法进行状态切换。
```
由于EFSM的巧妙设计，避免了命名冲突的问题，你可以在一个程序中定义多个状态机；要是能对不同状态进行组织，还可以做出层次状态机的结构。EFSM总共分为两个部分：

```text
- EFSM核心：由uthash.h、efsm.h和efsm_conf.h三个文件组成；他们构成了事件驱动型状态机的核心；使用的时候只需要包含efsm.h即可；
- EFSM扩展：在EFSM核心的基础上，增加efsmt.h和efsmt.c两个文件，这两个文件会根据具体的状态机创建状态机线程，用于驱动状态机运转；使用的时候只需要包含efsmt.h即可；
```

### <font color="red">4、WowCube - 具有24个屏幕的魔方游戏机</font>

WowCube是2021年CES创新奖的获奖者。这款立方体形状的设备由父子团队Savva和Ilya Osipov发明，两侧各有4个彩色IPS屏幕--总共24个，还有8个微处理器和隐藏在内部的加速计。

> 项目主页: https://wowcube.com/

![](http://henjay724.com/image/biweekly20210516/WowCube.PNG)

WowCube用户可以沿着多个轴转动从而不断改变屏幕之间的排列方式。游戏是通过旋转和摇晃设备来实现。用户无需点击屏幕或按键。

## 工具类

### <font color="red">1、爱科识 - 用于静态代码扫描（SAST）的下一代源代码分析工具</font>

爱科识是用于静态代码分析(SAST)的下一代源代码分析工具。它使用先进的编译 器分析技术来解析软件程序上下文、数据流及控制流，以便检测出代码里难以找出的缺陷。 爱科识能 轻松、快速地开发高质量代码、识别漏洞，并保证代码符合公司与行业，以及软件的合规性标准。

> 软件主页: https://xcalibyte.com.cn/aikeshi-jingtai-fenxi-gongju/

![](http://henjay724.com/image/biweekly20210516/aikeshi-flow.PNG)

爱科识精准、直观，可在软件开发生命周期（SDLC）的早期识别代码缺陷。您可以在开发周期中进行“左移”测试，从而极大地提高工作效率。此外，爱科识还可通过源代码分析来识别导致内存损坏，核心转储，缓冲区溢出，非法操作，空指针等的缺陷。

### <font color="red">2、ImHex - 一款功能强大的开源十六进制编辑器</font>

ImHex是一款功能强大的十六进制编辑器，该工具专为逆向工程分析师、编程开发人员以及那些想好好保护自己眼睛的安全人员所设计。

> 软件主页: https://github.com/WerWolv/ImHex

![](http://henjay724.com/image/biweekly20210516/ImHex.png)

功能包括：

```text
- 功能丰富的十六进制数据界面：字节修复、修复管理、字节拷贝（字节、十六进制字符串、C、C++、C#、Rust、Python、Java和JavaScript数组、HTML自包含div等）。
- 字符串、十六进制搜索。
- 自定义C++类模式语言，支持对文件内容进行解析和高亮显示。
- 数据导入：支持Base64文件、IPS和IPS32。
- 数据导出：IPS和IPS32。
- 数据检查器允许解释多种不同类型的数据（小端和大端）。
- 大文件支持和快速有效的加载。
- 文件哈希支持：CRC16、CRC32、MD4、MD5、SHA-1、SHA-224、SHA-256、SHA-384和SHA-512。
- 反汇编程序支持多种不同的体系结构：ARM32 (ARM, Thumb, Cortex-M, AArch32)、ARM64、MIPS (MIPS32, MIPS64, MIPS32R6, Micro)、x86 (16-bit, 32-bit, 64-bit)、PowerPC (32-bit, 64-bit)、SPARC、IBM SystemZ、xCORE、M68K、TMS320C64X、M680X和Ethereum。
- 支持书签、区域突出显示和注释。
- 数据分析：提供文件解析器和MIME类型数据库、字节分布图、熵图、最高平均熵、加密/压缩文件检测。
- 其他实用工具：ASCII表、正则表达式替换、数学表达式计算器、十六进制颜色选择器。
```

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

