# 痞子衡嵌入式半月刊： 第 59 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 58 期》](https://www.cnblogs.com/henjay724/p/16484199.html)

## 唠两句

历史上的今天：

本期共收录 2个项目、1个工具，希望对你有帮助！

## 项目类

### <font color="red">1、OpenSK - 基于 Rust 语言编写的安全密钥软件包</font>

OpenSK 是谷歌推出的基于 Rust 语言编写的安全密钥，同时支持 FIDO U2F 和 FIDO2 标准。该项目是为了推进和改善对 FIDO 身份验证器的实现。

> * 项目地址：https://github.com/google/OpenSK

OpenSK 项目选择了 Nordic 的 nRF52840 加密狗套件作为初始参考硬件，因为它支持 FIDO2 提到的所有主要传输协议：NFC，低功耗蓝牙，USB和专用硬件加密核心。为了保护和携带套件钥匙，还提供了保护套。

![](http://henjay724.com/image/biweekly20220730/OpenSK.PNG)

### <font color="red">2、WiPhone - 基于ESP32的开源模块化手机</font>

WiPhone 是一款可破解的模块化手机，可以通过 WiFi 免费拨打高清语音。WiPhone 不仅具有完全免费的通话功能，而且还是一个基于 Arduino 的开源平台。

> * 项目地址：https://wiphone.io/

WiPhone 可以通过子板进行扩展。整个手机背面是一个可更换的面板，接受1.6毫米厚度的标准PCB，你可以用它添加任何你喜欢的功能。

![](http://henjay724.com/image/biweekly20220730/WiPhone.PNG)

## 工具类

### <font color="red">1、TinyPNG - 在线智能压缩WebP/PNG/JPEG格式图片</font>

TinyPNG 使用智能有损压缩技术将 PNG 文件的文件大小降低。通过选择性的减少图片中的颜色，只需要很少的字节数就能保存数据。经过压缩后的图片对视觉的影响几乎不可见，但是在压缩后的文件大小上有非常大的差别。

> * 官网地址：https://tinypng.com/

官方的测试，一个是 PS 保存的 24 位 PNG，另一个是 TinyPNG 保存的，两者大小差别近 4 倍。有了这个网站，我们可以在嵌入式应用里多存储一些图片资源了。

![](http://henjay724.com/image/biweekly20220730/TinyPNG.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

