# 痞子衡嵌入式半月刊： 第 59 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 58 期》](https://www.cnblogs.com/henjay724/p/16484199.html)

## 唠两句

历史上的今天：1923年7月30日，中国自行设计生产的第一架双层螺旋桨敞盖飞机由广东飞机制造厂研制成功命名为“洛士文一号”。

本期共收录 5 个项目、1 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、OpenSBI - RISC-V SBI 规范的开源参考实现</font>

RISC-V 处理器架构中，存在着定义于操作系统之下的环境，它被称作 SBI 标准。这个环境除了引导系统启动，还将常驻后台，在内核运行时提供处理器功能。RISC-V Supervisor 二进制接口（SBI）是以下之间的推荐接口：

```text
1. 在 M 模式下运行的特定于平台的固件，以 S 模式或 HS 模式执行的引导加载程序，管理程序或通用 OS。
2. 在 HS 模式下运行的管理程序，以及在 VS 模式下执行的引导加载程序或通用 OS。
```

OpenSBI 项目的目标是为在 M 模式下执行的平台特定固件（上面提到的情况 1）提供 RISC-V SBI 规范的开源参考实现。 RISC-V 平台和片上系统供应商可以轻松扩展 OpenSBI 实现，以适应特定的硬件配置。

> * 项目地址：https://github.com/riscv-software-src/opensbi

OpenSBI 的主要组件以独立于平台的静态库 libsbi.a 的形式提供，实现了 SBI 接口。固件或引导加载程序实现可以链接到此库，以确保符合 SBI 接口规范。 libsbi.a 还定义了用于与平台固件实现提供的平台特定操作集成的接口（例如，控制台访问功能，处理器间中断控制等）。

### <font color="red">2、RustSBI - RISC-V SBI 规范的 Rust 实现</font>

RustSBI 是 RISC-V 平台下的引导程序实现，它完全由 Rust 编写，并已经被录入 RISC-V SBI 国际标准。

> * 项目地址：https://github.com/rustsbi/rustsbi

RustSBI 是一个扩展性较好的库，允许开发者自由地添加需要的功能模块，以支持芯片研发企业、应用厂商和板卡厂商提供自己芯片的 SBI 支持环境。

### <font color="red">3、OpenSK - 基于 Rust 语言编写的安全密钥软件包</font>

OpenSK 是谷歌推出的基于 Rust 语言编写的安全密钥，同时支持 FIDO U2F 和 FIDO2 标准。该项目是为了推进和改善对 FIDO 身份验证器的实现。

> * 项目地址：https://github.com/google/OpenSK

OpenSK 项目选择了 Nordic 的 nRF52840 加密狗套件作为初始参考硬件，因为它支持 FIDO2 提到的所有主要传输协议：NFC，低功耗蓝牙，USB和专用硬件加密核心。为了保护和携带套件钥匙，还提供了保护套。

![](http://henjay724.com/image/biweekly20220730/OpenSK.PNG)

### <font color="red">4、WiPhone - 基于ESP32的开源模块化手机</font>

WiPhone 是一款可破解的模块化手机，可以通过 WiFi 免费拨打高清语音。WiPhone 不仅具有完全免费的通话功能，而且还是一个基于 Arduino 的开源平台。

> * 项目地址：https://wiphone.io/

WiPhone 可以通过子板进行扩展。整个手机背面是一个可更换的面板，接受1.6毫米厚度的标准PCB，你可以用它添加任何你喜欢的功能。

![](http://henjay724.com/image/biweekly20220730/WiPhone.PNG)

### <font color="red">5、EEZ Bench Box 3 - 开源的模块化，可编程直流电源</font>

EEZ Bench Box 3 (BB3) 代表了模块化测试和测量(T&M)设备的一个新类别。它提供了一个完整的开源硬件和软件框架，弥合了DIY爱好者工具和专业台式设备之间的差距，并结合了最好的功能。

> * 旧版项目地址：https://www.crowdsupply.com/envox/eez-h24005
> * 新版项目地址：https://www.crowdsupply.com/envox/eez-bb3

BB3的灵感来自EEZ H24005电源，该电源以其广泛的功能集、丰富的用户界面、diy友好性和完全开源的设计吸引了许多爱好者。BB3最初将配备与H24005功能相同的模块，但这些模块将插入到设备中，提供更好的模块性、更大的容量、更强的处理能力、更容易使用的界面和更强的灵活性，所有这些都以紧凑的形式实现。

![](http://henjay724.com/image/biweekly20220730/EEZ-Bench-Box-3.PNG)

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

