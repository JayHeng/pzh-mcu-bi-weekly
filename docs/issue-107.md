# 痞子衡嵌入式半月刊： 第 107 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 106 期》](https://www.cnblogs.com/henjay724/p/18360229)

## 唠两句

历史上的今天：1999年9月8日，中国第一台交流传动内燃机车研制成功。

本期共 4 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、str - 一个方便直观的C字符串处理库</font>

这个项目旨在实现一种方便直观的字符串处理方法，灵感来自于 Luca Sas 的 YouTube 视频中的演讲。项目核心思想是将字符串的所有权(可以修改/构建字符串)与字符串的访问或视图(导航/分割/修剪)分离，按值返回字符串，以避免指针，并且放弃对 null 终止的要求。

 * 项目地址：https://github.com/mickjc750/str

项目特点包括：

```text
- 支持静态或堆栈分配缓冲区，适用于不能(或不愿意)使用动态内存分配的应用程序。
- 支持自定义分配器，适用于使用临时分配器提高速度的应用程序。为了简单起见，可以默认为malloc/free。
- 一套丰富的字符串分割/修剪/搜索功能。
- 一个数字解析器，用于检查错误，包括范围错误或无效输入。
```

### <font color="red">2、varch - 一个嵌入式C语言常用代码模块库</font>

varch（we-architecture，意为我们的框架库）是嵌入式 C 语言常用代码模块库，包含了嵌入式中常用的算法库, 数据结构（容器）库, 解析器库, 独立C语言 std 库, 工具库等等。具有简单, 通用, 高效的特点，目的为了学习以及在开发中拿来就用，提高开发效率以及代码可靠稳定性。

 * 项目地址：https://gitee.com/Lamdonn/varch

### <font color="red">3、letter-shell - 一个特别适用MCU的嵌入式小型shell</font>

letter shell 是一个 C 语言编写的，可以嵌入在程序中的嵌入式 shell，主要面向嵌入式设备，以 C 语言函数为运行单位，可以通过命令行调用，运行程序中的函数。  

相对经典的 2.x 版本，letter shell 3.x 增加了用户管理，权限管理，以及对文件系统的初步支持。此外 3.x 版本修改了命令格式和定义，2.x 版本的工程需要经过简单的修改才能完成迁移。

 * 项目地址：https://gitee.com/zhang-ge/letter-shell

letter shell 3.x 主要功能有：

```text
- 命令自动补全
- 快捷键功能定义
- 命令权限管理
- 用户管理
- 变量支持
- 代理函数和参数代理解析
```

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-107/shell_end_line_mode.gif)

### <font color="red">4、usb-sniffer-lite - 一个基于RP2040的USB2.0分析仪</font>

这是一个简单的基于树莓派 RP2040 的 USB 2.0 分析仪。它支持低速和全速模式。固件将自己呈现为虚拟 com 端口(VCP)，因此不需要额外的软件，并且它与所有操作系统兼容。

这个分析仪没有数据包解码功能，但是有一个优秀的在线 USB 描述符和请求解析器，它对解码标准描述符和请求非常有帮助。编译后的二进制文件需要更新 CRC 值才能被 RP2040 识别。这可以使用 bin2uf2 工具完成。  

 * 项目地址：https://github.com/ataradov/usb-sniffer-lite

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-107/usb-sniffer-lite.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

