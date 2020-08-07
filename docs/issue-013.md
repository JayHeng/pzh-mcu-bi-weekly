# 痞子衡嵌入式半月刊： 第 13 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 12 期》](https://www.cnblogs.com/henjay724/p/13363449.html)

## 唠两句

今天是立秋，立秋并不代表酷热天气就此结束，初秋期间天气仍然很热。

本期共收录 2条资讯、 个项目、2个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、全志将基于平头哥玄铁平台开发RISC-V芯片</font>

2018年阿里宣布成立平头哥半导体正式进军芯片设计领域。2019年7月，阿里正式推出了玄铁910处理器内核，号称业界最强RISC-V处理器，并对外开放授权。近日，全志科技宣布与阿里平头哥达成合作协议，将基于玄铁平台开发通用算力芯片。

全志和平头哥双方首款合作产品已经开始研发，即全志基于平头哥玄铁 902 处理器开发通用算力芯片，量产周期可进一步缩短，并且有望在功耗上实现新的突破，该芯片可应用于智能家居、工业控制及消费电子领域，预计3年出货5000万颗。未来，全志还将推出更多基于玄铁系列处理器的芯片。

![](http://henjay724.com/image/biweekly/t-head_E902_block_diagram.PNG)

### <font color="red">2、兆易创新发布中国首款Cortex-M33内核GD32E5系列MCU</font>

兆易创新GigaDevice 近日正式发布基于全新Arm® Cortex®-M33内核的GD32E5系列高性能微控制器。

作为中国第一个Arm® Cortex®-M33内核通用MCU，GD32E5系列为数据密集、算法密集、传输密集的高精度工控和消费类应用，提供了高性价比的解决方案。并将以持续拓展的GD32生态系统为服务支撑，深耕市场行业需求，提升用户开发体验。

![](http://henjay724.com/image/biweekly/GD32E5_Series.png)

GD32E5产品组合提供了3个通用系列和1个专用系列，4种封装类型23个型号选择，目前已经开始提供样片和开发板卡，并将于下个月正式投入量产。

## 项目类

### <font color="red">1、Air:bit - 用Micro:bit制作的无人机</font>

Air:bit是挪威的一个团队在Kickstarter上众筹的一个无人机，机身用Micro:bit制作，遥控器也通过Micro:bit板实现。

> 众筹主页： https://www.kickstarter.com/projects/makekit/airbit

![](http://henjay724.com/image/biweekly/air-bit.png)

![](http://henjay724.com/image/biweekly/air-bit-control.png)

## 工具类

### <font color="red">1、VSPD - 超级好用的虚拟串口软件</font>

为解决计算机的物理串口个数的限制，在进行串口调试实验时，应尽可能采用虚拟串口软件。VSPD（Virtual Serial Ports Driver）虚拟串口软件是由Eltima软件公司设计的虚拟串口软件，使用方便且稳定。

> 软件官网： https://www.virtual-serial-port.org/

使用虚拟串口也是规避风险的好办法，尤其对新手而言，应该先在虚拟串口环境下调试自己的代码，成功之后再连接物理串口，链接物理串口之前一定要检查连线是否正确，并用万能表检测是否有短路断路情况发生，否则极易烧毁串口。

![](http://henjay724.com/image/biweekly/Virtual_Serial_Port_Driver.PNG)

### <font color="red">2、Everything - 非常优秀的文件搜索软件</font>

Everything是voidtools开发的一款文件搜索工具，官网描述为“基于名称实时定位文件和目录”。它体积小巧，界面简洁易用，快速建立索引，快速搜索，同时占用极低的系统资源，实时跟踪文件变化，并且还可以通过http或ftp形式分享搜索。

> 软件官网： https://www.voidtools.com/

Everything可以说是速度最快的文件名搜索软件。其速度之快令人震惊，百G硬盘几十万个文件，可以在几秒钟之内完成索引，文件名搜索瞬间呈现结果。小巧免费，支持中文，支持正则表达式。

![](http://henjay724.com/image/biweekly/Everything.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)


