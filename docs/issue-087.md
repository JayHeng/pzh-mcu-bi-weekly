# 痞子衡嵌入式半月刊： 第 87 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 86 期》](https://www.cnblogs.com/henjay724/p/17872180.html)

## 唠两句

历史上的今天：。

本期共收录 1 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、Ethersweep - 开源以太网可控步进电机</font>

Ethersweep 是 NEMA17 步进电机的电机控制器，可以从普通以太网网络来控制。我们可以从任何机器发送 UDP 消息来控制电机，也可以控制多个电机，因为每个电机从网络上的 DHCP 服务器获得一个 IP 地址。此外还可以将 End-stop 和 e-stop 连接到控制器。传感器数据，如编码器反馈，电压，运行和按钮状态也可以通过网络请求来请求。

 * 项目地址：https://github.com/neumi/ethersweep

Ethersweep 主要硬件包括：

```text
W5500 Ethernet controller
STM32F103 Microcontroller @ 72MHz
Trinamic TMC2209 Stepper motor driver
AS5600 magnetic rotary encoder
```

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-087/Ethersweep.PNG)

## 工具类

### <font color="red">1、SWIG - 将C/C++程序转换成其他高级编程语言</font>

SWIG 能够将用 C 和 C++ 编写的程序转换成各种高级编程语言。包括常见的脚本语言，如 Javascript、Perl、PHP、Python、Tcl和Ruby。还支持非脚本语言，如 C#、D语言、Go语言、Java(包括Android)、Lua、OCaml、Octave、Scilab和 R。还支持一些解释和编译的Scheme实现(Guile、MzScheme/Racket)。

 * 工具地址：https://www.swig.org/

SWIG 最常用于创建高级解释或编译的编程环境、用户界面，并作为测试和原型化 C/C++ 软件的工具。SWIG 通常用于解析 C/C++ 接口，并生成上述目标语言调用到 C/C++ 代码所需的“粘合代码”。SWIG 还可以以 XML 的形式导出其解析树。

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

