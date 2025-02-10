# 痞子衡嵌入式半月刊： 第 117 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 116 期》](https://www.cnblogs.com/henjay724/p/18666052)

## 唠两句

历史上的今天：1996年2月10日，IBM开发的深蓝计算机首次挑战国际象棋世界冠军卡斯帕罗夫，最终以2:4落败。

本期共 3 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、ztask - 一个简单的基于计时器的调度器</font>

ztask 是一个简单的基于计时器的调度器，除了 C 语言版本之外，也提供了 C++ 版本。C 语言版本就 ztask.h 和 ztask.c 俩文件，五个 API。使用方法: 定义任务函数, 在进入主循环前执行 zt_bind 即可。之后在主循环里调用 zt_poll(), 在 systick 中断里调用 zt_tick() 就行了。如果需要控制任务启动/停止，需要用一个变量保存 zt_bind 的返回值，然后执行 zt_start 和 zt_stop。

 * 项目地址：https://github.com/tomzbj/ztask

因为 ztask 只是调度器，不是 OS，不支持抢占，所以要用户自己保证任务在短时间内退出，不会长期占用。许多 GUI 或者 OS 框架之类的内置调度器其实原理都差不多。

### <font color="red">2、CDNET - 面向CDBUS的可选高层协议</font>

传统串口协议很多，但是都不是很理想，譬如解析 AT 命令很麻烦、MODBUS 只支持单方向查询、PPP 协议要转义、字符串协议效率低。CDNET 协议非常简单，可以支持数据表读写、打印、IAP、波形显示 等功能，还可以使用配套开源上位机 cdbus_gui、cdnet_tun 等工具，把简单的串口数据包映射成电脑 UDP 数据包，上位机可以使用 UDP/IP 实现串口通讯，且解决了同一时间一个串口只能被一个软件打开的限制。

 * 项目地址：https://github.com/dukelec/cdnet

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-117/CDNET.png)

### <font color="red">3、MiaoUI - 一个基于C语言的单色OLED菜单UI框架</font>

MiaoUI 是一个基于 u8g2 的单色 OLED 菜单 UI 框架。MiaoUI使用 C 语言实现，采用双向链表结构，使用非线性动画、移植方便、内存占用较小、能够快速部署，适用于具有小型 OLED 屏幕的嵌入式设备。

 * 项目地址：https://github.com/JFeng-Z/MiaoUI

MiaoUI 主要特点如下：

```text
- 多样化的菜单类型：支持 列表类菜单 和 图标类菜单，满足不同应用场景。
- 流畅动画效果：内置 非线性动画，可动态打断，提升用户体验。
- 灵活的自定义功能：支持菜单项自定义，列表与图标菜单可灵活嵌套。
```

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-117/MiaoUI.png)

## 工具类

### <font color="red">1、OpenEPT - 开源低功耗测试仪</font>

OpenEPT 的主要目标是为工程师和研究人员提供一套全面的微控制器分析工具，促进对基于微控制器平台功耗的准确分析。所有资料全开源，还有一个上位机，方便查看功耗波形。

 * 项目地址：https://www.openept.net/

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-117/OpenEPT1.png)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-117/OpenEPT2.png)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

