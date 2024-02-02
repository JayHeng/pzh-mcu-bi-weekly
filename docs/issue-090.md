# 痞子衡嵌入式半月刊： 第 90 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 89 期》](https://www.cnblogs.com/henjay724/p/17964146)

## 唠两句

历史上的今天：1982年1月14日，中国成功完成酵母菌丙氨酸转移核糖核酸的人工全合成。

本期共收录 2 个项目、0 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、TFT_eSPI - 一个功能强大的TFT屏驱动库</font>

TFT_eSPI 是一个为 MCU 设计且兼容 Arduino IDE 的图形和字体库，它已针对 RP2040, STM32, ESP8266 和 ESP32 类 MCU 进行了性能优化，当然也可以配合其他 32 位处理器使用，但将使用较慢的通用 Arduino 接口调用。

该库可以使用 Arduino IDE 的库管理器加载。直接内存访问(DMA)可以与 ESP32, RP2040和STM32 处理器一起使用，带有 SPI 接口显示器，以提高渲染性能。具有并行接口(8位和16位)的 DMA 仅支持RP2040。

 * 项目地址：https://github.com/Bodmer/TFT_eSPI

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-090/TFT_eSPI.jpg)

### <font color="red">2、LovyanGFX - 又一个功能完善的TFT屏驱动库</font>

LovyanGFX 是一个为 MCU 设计的 TFT 图形驱动库，底层主要适配 ESP32 SPI, I2C, 8bitParallel / ESP8266 SPI, I2C / ATSAMD51 SPI，同时支持非常多的 LCD 驱动芯片。  

LovyanGFX 主要特点包括：

```
- 支持ArduinoESP32和ESP-IDF。
- 支持16位和24位颜色模式。(实际颜色数量视显示器规格而定)
- 在使用DMA传输的通信操作期间执行另一个进程。
- 快速旋转/扩展屏幕外缓冲区。
- 同时使用多个显示器。
- 单色显示器彩色还原图的自动处理。
- OpenCV,SDL2可以用作绘图目标，并且可以在PC上运行。
- 复合视频信号(NTSC, PAL)输出(仅ESP32)
```

 * 项目地址：https://github.com/lovyan03/LovyanGFX

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-090/LovyanGFX.jpg)

## 工具类



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

