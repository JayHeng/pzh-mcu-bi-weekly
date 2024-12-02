# 痞子衡嵌入式半月刊： 第 112 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 111 期》](https://www.cnblogs.com/henjay724/p/18551164)

## 唠两句

Linus Torvalds 是非常厉害的程序员，他有两个名扬天下的作品：Linux 和 Git。但如果单论技术能力，有一个人也许比 Linus 更强，他就是法国程序员 Fabrice Bellard。本期项目均出自 Fabrice Bellard，他的博客 [bellard.org](https://bellard.org/) 有很多很棒的开源项目。

本期共 3 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、TinyGL - 一个轻量级的OpenGL库实现</font>

TinyGL 是 OpenGL 的一个小型实现，适用于嵌入式系统。TinyGL 的核心是将复杂的 OpenGL 接口精简为更易于理解和操作的形式。它并不旨在替换完整的 OpenGL 库，而是一个教学工具和实验平台，特别是在嵌入式系统或者对性能要求不那么严苛的场景中。

 * 项目地址：https://bellard.org/TinyGL/

TinyGL 基于原始的 OpenGL 规范，但进行了大幅简化。它包含了基本的几何绘制、颜色设定、视口管理和变换等功能。主要特性包括：

```text
基本绘图：支持点、线和多边形的绘制。
颜色管理：可以设置颜色模式，包括单色和RGB颜色。
视口和投影：可以调整视口大小和定义投影矩阵。
变换操作：支持平移、旋转和缩放等基本几何变换。
```

### <font color="red">2、FFmpeg - 一个完整的跨平台音视频处理框架</font>

FFmpeg 是广泛使用的多媒体解决方案，既是一款音视频编解码工具，同时也是一组音视频编解码开发套件，作为编解码开发套件，它为开发者提供了丰富的音视频处理的调用接口。其包括了目前领先的音/视频编码库 libavcodec。FFmpeg 提供了多种媒体格式的封装和解封装，包括多种音视频编码，多种协议的流媒体，多种色彩格式转换，多种采样率转换，多种码率转换等。FFmpeg 发展至今，已经被许多开源项目使用。

 * 项目地址：https://ffmpeg.org//

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-112/FFmpeg.PNG)

### <font color="red">3、TCC - 一个体积小巧但功能完整的C语言编译器</font>

Tiny C Compiler（TCC）是一个开源的 C 语言编译器项目，旨在创建一个体积小巧但功能完整的 C 语言编译器。随着技术的发展，TCC 已经成为了许多开发者和研究者进行编译器学习和研究的首选工具。

TCC 的特点是快速编译和小巧的体积，它支持标准  C语言（ISO C99），并且可以在多种操作系统上运行，包括 Linux、Windows、Mac OS X 等。由于其轻量级的特性，TCC 非常适合于嵌入式系统、教学和简单的项目。尽管它的功能和性能无法与 GCC 或 Clang 等大型编译器相比，但它在快速原型设计和学习领域中的应用尤为突出。 

 * 项目地址：https://bellard.org/tcc/


### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

