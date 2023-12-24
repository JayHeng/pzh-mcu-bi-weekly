# 痞子衡嵌入式半月刊： 第 88 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 87 期》](https://www.cnblogs.com/henjay724/p/17893196.html)

## 唠两句

历史上的今天：1906年12月24日，美国无线电爱好者费森登首次在世界上进行了无线电广播。

本期共收录 4 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、ethernet-to-spi - 以太网10BASE-T转SPI硬件实现</font>

这个项目的想法是将曼彻斯特编码的 10BASE-T 信号转换为 SPI，并使用 STM32F401 MCU 对其进行解析。项目使用 75C1168 芯片将差分信号转换为 5V 逻辑电平，然后使用 74HC86 XOR 检测边缘。项目的原理图，PCB，固件全开源。

 * 项目地址：https://github.com/imihajlow/ethernet-to-spi

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-088/ethernet-to-spi.PNG)

### <font color="red">2、RoenDi - 带TFT显示的开源旋转编码器</font>

RoenDi 是一个视觉适应性强的旋转编码器，能够显示定制的图形。有一个内置的屏幕允许它提供视觉反馈，不像任何其他我们见过的编码器。RoenDi 的设计思路是简单和多功能性，只需连接 microrousb 电缆或 ST-LINK 连接器，将代码上传到 MCU，就可以开始了。

 * 项目地址：https://github.com/MitkoDyakov/Roendi

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-088/RoenDi.PNG)

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-088/RoenDi2.PNG)

### <font color="red">3、Marlin - 基于Arduino平台的RepRap 3D打印机优化固件</font>

Marlin 是一个开源固件，用于复制快速原型机的 RepRap 家族-通常被称为“3D打印机”。它源自于Sprinter 和 grbl，并于2011年8月12日在Github上发布，成为一个独立的开源项目。

从一开始，Marlin就是由RepRap爱好者构建的，它是一个简单、可靠、适应性强的打印机驱动程序，“只是工作”。作为其质量的证明，Marlin被几个受人尊敬的商业3D打印机使用。LulzBot, Průša Research, Creality3D, BIQU, Geeetech和Ultimaker只是一些提供Marlin变体的供应商。Marlin还能驾驶数控机床和激光雕刻机。

 * 项目地址：https://github.com/MarlinFirmware/Marlin

Marlin受欢迎的一个关键是它运行在便宜的8位Atmel AVR微控制器- Marlin 2上。X增加了对32位板的支持。这些芯片是流行的开源Arduino/Genuino平台的核心。Marlin的参考平台是带有RAMPS 1.4的Arduino Mega2560和带有RAMPS 1.4的rearm。

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-088/Marlin.PNG)

### <font color="red">4、esp_ghota - 从Github版本更新esp32固件的OTA组件</font>

这个项目可以帮助自动化 OTA 和 CI/CD 管道，其可以直接从 Github 版本发布来更新 ESP32 芯片。

 * 项目地址：https://github.com/Fishwaldo/esp_ghota

esp_ghota 特性包括：

```text
- 使用底层的esp_htps_ota库来更新固件映像
- 还可以更新spiffs/littlefs/fatfs分区
- 使用SemVer比较版本，仅在有新版本可用时更新
- 与esp-idf引导加载程序的应用程序回滚和反回滚功能配合得很好
- 直接从github发布页面下载固件和分区映像
- 支持使用不同固件映像的多个设备
- 包括一个示例Github动作，当一个新的标签被推送时，构建和释放图像
- 更新可以手动触发，也可以通过间隔计时器触发
- 使用流JSON解析器来减少内存使用(Github API响应可能很大)
- 支持私有存储库(需要Github API令牌)
- 支持Github企业
- 支持Github个人访问令牌，以克服Github API速率限制
- 通过esp_event_loop发送更新的进度
```

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

