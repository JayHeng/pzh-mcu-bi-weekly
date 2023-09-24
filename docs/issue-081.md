# 痞子衡嵌入式半月刊： 第 81 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 80 期》](https://www.cnblogs.com/henjay724/p/17711448.html)

## 唠两句

历史上的今天：1909年9月24日，由中国工程师詹天佑自行设计组织建造的京张铁路建成通车。

本期共收录 3 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、mcu_bsdiff_upgrade - 适用于嵌入式单片机的差分升级通用库</font>

mcu_bsdiff_upgrade 是一款适用于嵌入式单片机的差分升级库，通用所有单片机，如stm32、华大、复旦微、瑞萨等。适合嵌入式的差分升级又叫增量升级，顾名思义就是通过差分算法将源版本与目标版本之间差异的部分提取出来制作成差分包，然后在设备通过还原算法将差异部分在源版本上进行还原从而升级成目标版本的过程。 差分升级方案不仅可以节省MCU内部的资源空间、还可以节省下载流程及下载和升级过程中的功耗。

mcu_bsdiff_upgrade 差分升级过程：

```text
1. 使用旧版本bin文件和新版本bin文件制作差分包
2. 将差分包下载到设备内
3. 设备使用差分算法还原出新版本bin
4. 设备将新版本bin进行crc验证后刷到代码执行区
5. 设备重启并以新版本运行
```

> * 项目地址：https://gitee.com/qq791314247/mcu_bsdiff_upgrade

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-081/mcu_bsdiff_upgrade.PNG)

### <font color="red">2、ESP32-Paxcounter - Wifi和BLE驱动的乘客流量测量仪</font>

Paxcounter是一个 proof-of-concept 设备，用于实时测量客流，它计算周围有多少移动设备，这可以估计出周围有多少人。Paxcounter检测空中的Wifi和蓝牙信号，通过过滤MAC地址中的供应商oui来关注移动设备。

这个项目的目的是在不侵犯隐私的情况下做到这一点：如果你只想统计用户拥有的设备，你不需要跟踪他们。因此，Paxcounter不会持久地存储MAC地址，也不会对扫描的设备进行指纹识别。数据通过LoRaWAN网络和/或有线SPI从接口传输到服务器。它也可以存储在本地SD-card上。

> * 项目地址：https://github.com/cyberman54/ESP32-Paxcounter

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-081/ESP32-Paxcounter.PNG)

### <font color="red">3、FindMyCat - 基于NRF9160的全开源宠物跟踪器</font>

FindMyCat 是一款电池寿命长达数月 (Near Home 模式下，待机功耗18uA，350mA电池，可工作2年)，可在室外和室内工作的开源宠物跟踪器。从原理图，PCB，Gerber Files，软件，IOS APP程序都非常完善的一个全开源项目。

FindMyCat 主要特点：

```text
- 使用定位技术，可以在LTE网络覆盖的地方定位你的宠物的位置。
- 使用苹果的近距离交互框架，蓝牙低功耗和超宽带技术（UWB），可以精确地找到你的宠物的位置，误差只有10厘米。
- 它有一个智能绑定功能，当你的宠物在家里时，它会和FindMyCat HomeStation建立一个虚拟的绳索，这样可以让GPS和LTE功能进入深度睡眠状态，节省电量，并通过家庭wi-fi发送位置更新。
- 它的电池可以持续6个月，比90%的商业产品都要长。
- 完全开源，你可以自己制作或者修改它。
```

> * 项目地址：https://github.com/FindMyCat/

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-081/FindMyCat.PNG)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-081/FindMyCat-Arch.PNG)

## 工具类

### <font color="red">1、grep - 超强的代码片段搜索工具</font>

grep 是一个超强的代码片段搜索工具，利用 grep 可以快速的在全球各大主流 GitHub 存储库中搜索代码片段或现有实现以供参考。

> * 工具地址：https://grep.app/

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-081/grep.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

