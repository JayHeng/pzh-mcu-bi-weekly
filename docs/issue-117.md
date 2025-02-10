# 痞子衡嵌入式半月刊： 第 117 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 116 期》](https://www.cnblogs.com/henjay724/p/18666052)

## 唠两句

历史上的今天：

本期共 1 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、ztask - 一个简单的基于计时器的调度器</font>

ztask 是一个简单的基于计时器的调度器，除了 C 语言版本之外，也提供了 C++ 版本。C 语言版本就 ztask.h 和 ztask.c 俩文件，五个 API。使用方法: 定义任务函数, 在进入主循环前执行 zt_bind 即可。之后在主循环里调用 zt_poll(), 在 systick 中断里调用 zt_tick() 就行了。如果需要控制任务启动/停止，需要用一个变量保存 zt_bind 的返回值，然后执行 zt_start 和 zt_stop。

 * 项目地址：https://github.com/tomzbj/ztask

因为 ztask 只是调度器，不是 OS，不支持抢占，所以要用户自己保证任务在短时间内退出，不会长期占用。许多 GUI 或者 OS 框架之类的内置调度器其实原理都差不多。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-117/.png)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

