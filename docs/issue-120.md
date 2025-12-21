# 痞子衡嵌入式半月刊： 第 120 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 119 期》](https://www.cnblogs.com/henjay724/p/19117426)

## 唠两句

最近看到国产半导体竞相推出高性能MCU产品，已经在多个垂直应用领域正面挑战国外巨头，不禁感慨行业发展之快。举个最典型的例子，国内AI眼镜正处于百厂大战阶段，看似非常激烈，但有一家国产半导体却稳坐钓鱼台，因为大家的眼镜几乎都采用他们家的MCU方案，你们能猜到是谁吗？  

本期共 1 条资讯，3 个项目，希望对你有帮助！

## 资讯类

### <font color="red">1、兆易创新推出新一代性能旗舰GD32H78D</font>

兆易创新近日推出 [GD32H78D/77D系列](https://www.gigadevice.com.cn/product/mcu/high-performance-mcus/gd32h7xx-series/gd32h78dh77d) 高性能32位通用微控制器，产品基于高性能Arm® Cortex®-M7内核，主频高达750MHz，配备高速大容量内存架构及640KB可与CPU同频运行紧耦合内存（TCM），搭载专用数学加速引擎及丰富的外设接口，实现了高性能、低功耗与专用加速器的完美融合。该系列MCU全新集成MIPI DSI接口，提供出色的多媒体处理能力，广泛适用于高端嵌入式HMI、手持云台、专业声卡、便携医疗设备、智能家居等丰富人机交互场景，为高性能嵌入式系统提供全面可靠的硬件平台。

 * 资讯来源：https://www.gigadevice.com.cn/about/news-and-event/news/gigadevice-launches-gd32h78d-77d-series-mcu

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-120/GD32H78D.png)

## 项目类

### <font color="red">1、LwOW - 适用于嵌入式的轻量级单总线协议库</font>

LwOW 是一个功能强大、轻量高效且易于使用的 OneWire 协议库。它支持 UART 和 GPIO 两种通信方式，并提供 DMA 加速和线程安全 API，以满足不同嵌入式系统的需求。其平台无关性和丰富的特性，使其成为嵌入式系统开发中理想的 OneWire 解决方案。无论您是需要在资源受限的微控制器上实现 OneWire 通信，还是需要在高性能系统中进行高效的数据采集，LwOW 都能为您提供可靠且高效的支持。

 * 项目地址：https://github.com/MaJerle/lwow

LwOW 还包含如下功能：

```text
- 原生DS18B20支持:直接支持流行的DS18B20温度传感器，无需额外配置。
- 线程安全API:提供线程安全的API，确保在多线程环境下也能稳定运行。
- 灵活的位操作API:提供精细的位操作API，方便用户进行更底层的控制。
- 设备扫描和识别:内置设备扫描和识别功能，轻松发现并管理OneWire网络上的设备。
- 多驱动程序支持:支持多种不同的设备驱动程序，方便用户扩展和定制。
```

### <font color="red">2、i2cdevlib - 为I2C设备设计的大一统抽象库</font>

i2cdevlib 是一组结构大体统一且文档完善的类，用于为 I2C 设备提供简单直观的接口。每个设备类都基于通用的 “I2Cdev” 类构建，该类将 I2C 的位级和字节级通信从具体设备类中抽象出来，使设备类保持简洁，同时只需修改一个类即可将 I2C 通信代码移植到不同平台（如 Arduino、PIC、MSP430、Jennic、简单的位操作等）。设备类的设计目标是完整覆盖每个设备文档中描述的所有功能，并提供一些通用的便利函数。

 * 项目地址：https://github.com/jrowberg/i2cdevlib

### <font color="red">3、lwext4 - 为微控制器提供的Ext2/3/4文件系统</font>

lwext4 是一个功能强大、高效且易于使用的微控制器 Ext2/3/4 文件系统。其支持多种特性、多种架构和多种编译环境，为嵌入式系统开发提供了极大的便利。通过灵活的配置和优化的性能，lwext4 能够满足不同嵌入式应用场景的需求，是构建可靠、高效的嵌入式存储系统的理想选择。

 * 项目地址：https://github.com/gkostka/lwext4

lwext4 有如下特点：

```text
- 文件类型：常规文件、目录、软链接
- 支持硬链接
- 支持多种块大小：1KB、2KB、4KB … 64KB
- 支持小端/大端架构
- 支持多种配置（ext2/ext3/ext4）
- 仅依赖 C 标准库
- 支持多种 CPU 架构（x86/64、Cortex-M 系列、MSP430 …）
- 内存占用小
- 配置灵活
```

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

