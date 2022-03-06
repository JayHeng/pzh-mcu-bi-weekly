# 痞子衡嵌入式半月刊： 第 50 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 49 期》](https://www.cnblogs.com/henjay724/p/15889994.html)

## 唠两句

昨天是惊蛰，历史上的今天：2017年3月6日，“海翼”号水下滑翔机刷新世界纪录，最大下潜深度达到6329米。

本期共收录 0个资讯、3个项目、1个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、</font>



![](http://henjay724.com/image/biweekly20220306/.PNG)

## 项目类

### <font color="red">1、X-TRACK - 一款开源GPS自行车码表</font>

X-TRACK 是一款开源 GPS 自行车码表，拥有可显示实时位置的离线地图，支持记录和显示实时轨迹以及导出标准GPX格式的轨迹文件。据网友粗略估算这个码表的硬件成本大概不到 300 元。

> * 项目地址：https://github.com/FASTSHIFT/X-TRACK

X-TRACK软件架构示意图如下：由HAL、Framework 和 APP 三层组成，Framework为核心。HAL层负责底层芯片驱动和传感器原始数据获取；Framework又包括三个模块，分别负责图形渲染、页面生命周期管理和消息分发处理。其中消息框架模块提供数据的分发和处理。

![](http://henjay724.com/image/biweekly20220306/X-TRACK-arch.PNG)

![](http://henjay724.com/image/biweekly20220306/X-TRACK.gif)

### <font color="red">2、Daytripper - 激光绊脚器（智能摸鱼神器）</font>

最近发现一个好玩的开源项目 Daytripper。有了它，再也不用担心摸鱼的时候被人发现了。Daytripper 其实是一个激光绊脚器，在接收到触发信号时：

```text
• 可以隐藏你的电脑桌面应用
• 锁定电脑屏幕
• 可以执行定制化脚本，完成任何你想做的事情
```

> * 项目地址：https://github.com/dekuNukem/daytripper

该项目包括主要包括两部分：

```text
• 发送器。负责运动检测，发送信号给接收器。
• 接收器。负责接收信号，转发给 PC。
```

![](http://henjay724.com/image/biweekly20220306/Daytripper.jpg)

![](http://henjay724.com/image/biweekly20220306/Daytripper.gif)

### <font color="red">3、the-little-bili-tv - 基于ESP32的哔哩哔哩小电视</font>

这款哔哩哔哩小电视采用 esp32 作为主控，lvgl GUI 界面设计，基于 idf4.0 开发 支持 smartconfig 或微信 airkiss 配网，功能包括：网络连接显示、网络获取时间、天气显示、温湿度采集、粉丝数显示、mqtt温湿度上传等。所有软硬全部开源。  

> * 项目地址：https://gitee.com/wangpeng25/the-little-bili-tv

![](http://henjay724.com/image/biweekly20220306/the-little-bili-tv.jpg)

## 工具类

### <font color="red">1、Ghidra - 开源软件逆向工程（SRE）框架</font>

Ghidra 是由美国国家安全局（NSA，National Security Agency）的研究理事会为 NSA 的网络安全任务开发的软件逆向工程（SRE）框架，它有助于分析恶意代码和病毒等恶意软件，并可以让网络安全专业人员更好地了解其网络和系统中的潜在漏洞。

> * 项目主页：https://github.com/NationalSecurityAgency/ghidra

Ghidra 特性如下：

```text
1. 包含了一套软件分析工具，用于分析各种平台上的编译代码，包括 Windows、macOS 和 Linux。
2. 功能包括反汇编、汇编、反编译、图形和脚本执行，以及数百个其它功能。
3. 支持各种处理器指令集和可执行格式，可以在用户交互和自动模式下运行。
4. 用户可以使用公开的 API 开发自己的 Ghidra 插件组件与脚本。
```

![](http://henjay724.com/image/biweekly20220306/Ghidra.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

