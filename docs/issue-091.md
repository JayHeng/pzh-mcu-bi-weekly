# 痞子衡嵌入式半月刊： 第 91 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 90 期》](https://www.cnblogs.com/henjay724/p/18004182)

## 唠两句

历史上的今天：。

本期共收录 5 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、C4 - 4个函数实现的C语言编译器</font>

C4 是用 4 个函数实现的 C 语言编译器。该项目仅用了 500+ 行代码、4 个函数，就实现了一个小型 C 语言编译器。但因为它的代码过于精简，所以源码阅读起来并不轻松。  

 * 项目地址：https://github.com/rswier/c4

### <font color="red">2、SDS - 简单的C语言动态字符串库</font>

SDS 是 Redis 作者写的 C 语言动态字符串。它相较于 C 字符串，使用起来更加方便。具有速度快(常数复杂度获取字符串长度)、二进制安全(图片、音频等)、兼容部分 C 字符串函数等特点。  

 * 项目地址：https://github.com/antirez/sds

```C
sds mystring = sdsnew("Hello World!");
printf("%s\n", mystring);
sdsfree(mystring);

output> Hello World!
```

### <font color="red">3、foolrenderer - C语言从零实现的软件渲染器</font>

foolrenderer 是用 C 语言从零实现的软件渲染器。不用图形 API 仅用几千行 C 代码，实现了一套类似 OpenGL 的基本图形功能，以及应用于游戏开发的实时渲染技术，如阴影、切线空间法线映射、基于物理的材质系统等。该项目包含丰富的注释和数学计算推导过程的说明，可用于帮助理解和学习 GPU 的基本工作原理、基础渲染知识和着色器原理。  

 * 项目地址：https://github.com/antirez/sds

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-091/foolrenderer.gif)

### <font color="red">4、Genann - 纯C实现的简单神经网络库</font>

Genann 是一个经过精心测试的库，用于在 C 中训练和使用前馈人工神经网络（ANN）。它的主要特点是简单、快速、可靠和可魔改（hackable），它只需要提供一些必要功能和一点额外功能就能实现这些。  

 * 项目地址：https://github.com/codeplea/genann

Genann 特点包含：

```text
- 没有依赖关系的ANSI C。
- 包含在一个单一的源代码和头文件。
- 简单，快速，线程安全，易于扩展。
- 实现反向传播训练。
- 兼容其他训练方法(经典优化、遗传算法等)
- 包括示例和测试套件。
- 在zlib许可下发布-几乎免费用于任何用途。
```

### <font color="red">5、excelCPU - 在Excel中构建出的16位CPU</font>

excelCPU 是一位业余爱好者通过 Excel 创建的一个 16 位 CPU。它在 Excel 中构建，以 3Hz 时钟频率运行，并具有 128KB RAM、16 色 128x128 像素显示屏和自定义汇编语言 Excel-ASM16。  

 * 项目地址：https://github.com/InkboxSoftware/excelCPU

这个 Excel CPU 项目中最令人印象深刻的壮举是 Excel-ASM16。这种汇编语言包含 23 种不同的指令，并支持变量、标签，甚至二进制文件支持。这些是汇编语言的基本功能，但足以满足在Microsoft Excel 下运行的 16 位 CPU 的限制。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-091/excelCPU.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

