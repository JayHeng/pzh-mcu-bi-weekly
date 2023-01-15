# 痞子衡嵌入式半月刊： 第 70 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 69 期》](https://www.cnblogs.com/henjay724/p/17010967.html)

## 唠两句

历史上的今天：2001年1月15日，维基百科，一个基于Wiki技术的多语言百科全书正式成立上线。

本期共收录 3 个工具、2 个RT产品，希望对你有帮助！

## 工具类

### <font color="red">1、CODESYS - 一款工业自动化领域的一款开发编程系统</font>

CODESYS 是一款工业自动化领域的一款开发编程系统，应用领域涉及工厂自动化、汽车自动化、嵌入式自动化、过程自动化和楼宇自动化等等。CODESYS 软件可以分为两个部分，一部分是运行在各类硬件中的RTE（Runtime Environment），另一部分是运行在PC机上的IDE。因此CODESYS的用户既包括生产PLC、运动控制器的硬件厂商，也包括最终使用PLC、运动控制器的用户。

> * 工具官网：https://www.codesys.com/

![](http://henjay724.com/image/biweekly20230115/CODESYS.PNG)

### <font color="red">2、Beremiz - 用于机械自动化的 PLC 集成开发环境</font>

Beremiz 是一个用于机械自动化的 PLC 集成开发环境（IDE），符合 IEC61131-3 编程语言标准，可将任何处理器变成 PLC。Beremiz 还包含用于创建 HMI 并将 PLC 程序连接到现有的监控、数据库或现场总线的工具。

> * 工具官网：https://beremiz.org/

Beremiz 由两部分组成：

```text
- 集成开发环境（IDE），Beremiz.py。它运行在用户的计算机上，使用 C 代码作为中间语言，用于编写、编译、调试 PLC 程序和控制 PLC 运行时。
- 引用 python 运行时实现，Beremiz_service.py，它在目标平台上运行，与 I/O 通信并执行 PLC 程序。
```

![](http://henjay724.com/image/biweekly20230115/Beremiz.PNG)

### <font color="red">3、JSON Crack - 一款非常优雅的 JSON 数据可视化工具</font>

JSON Crack 是一个很方便的 JSON 数据可视化工具。 该项目不是简单的展示 JSON 数据,而是将其转化为类似思维导图的形式,支持放大/缩小、展开/收缩、搜索节点、导出图片等操作。对于经常和json格式的数据打交道的人会非常有帮助。 

> * 工具官网：https://jsoncrack.com/

![](http://henjay724.com/image/biweekly20230115/JSONCrack.PNG)

## i.MXRT出品

### <font color="red">1、佳明 - 智能手表 Enduro 2</font>

GARMIN 安夺 Enduro 2专为极限耐力运动员打造，采用轻量化防刮类钻碳镀膜钛合金表圈及后壳，搭载 1.4 英寸恒亮屏幕，全新触控屏。腕表内预装中国大陆导航详图及全球雪道图、全球高尔夫球场图等，多频多星系统结合 SatIQ 科技。

> * RT芯片：i.MXRT595
> * 产品主页： https://www.garmin.com/en-US/p/854515
> * 官网定价： 999 美元起

![](http://henjay724.com/image/biweekly20230115/Enduro2.PNG)

### <font color="red">2、大疆创新 - 运动相机（Action 2双屏套装）</font>

DJI Action 2 是新一代磁吸式運動相機,多種形態自由切換,既可以手持或穿戴,也能粘附固定拍攝。具備旗艦拍攝性能,支援4K/120fps影片,155° 超廣角,防水耐摔,助你輕鬆玩轉全場。

> * RT芯片：i.MXRT1064
> * 产品主页： https://www.dji.com/cn/dji-action-2?from=store-product-page
> * 官网定价： 3499 元起

![](http://henjay724.com/image/biweekly20230115/Action2.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

