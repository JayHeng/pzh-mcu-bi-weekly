# 痞子衡嵌入式半月刊： 第 88 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 87 期》](https://www.cnblogs.com/henjay724/p/17893196.html)

## 唠两句

历史上的今天：。

本期共收录 2 个项目、0 个工具，希望对你有帮助！

## 项目类

### <font color="red">1、ethernet-to-spi - 以太网10BASE-T转SPI硬件实现</font>

这个项目的想法是将曼彻斯特编码的 10BASE-T 信号转换为 SPI，并使用 STM32F401 MCU 对其进行解析。项目使用 75C1168 芯片将差分信号转换为 5V 逻辑电平，然后使用 74HC86 XOR 检测边缘。项目的原理图，PCB，固件全开源。

 * 项目地址：https://github.com/imihajlow/ethernet-to-spi

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-088/ethernet-to-spi.PNG)

### <font color="red">2、esp_ghota - 从Github版本更新esp32固件的OTA组件</font>

这个项目可以帮助自动化 OTA 和 CI/CD 管道，其可以直接从 Github 版本发布来更新 ESP32 芯片。

 * 项目地址：https://github.com/Fishwaldo/esp_ghota

esp_ghota 特性包括：

```
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

## 工具类

### <font color="red">1、</font>



### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

