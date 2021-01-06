# 痞子衡嵌入式半月刊： 第 23 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 22 期》](https://www.cnblogs.com/henjay724/p/14175100.html)

## 唠两句

昨天是小寒。

本期共收录 0条资讯、0个项目、1个工具，希望对你有帮助！

## 资讯类

### <font color="red">1、</font>


![](http://henjay724.com/image/biweekly/.png)

## 项目类

### <font color="red">1、</font>



## 工具类

### <font color="red">1、TinyGo - 基于LLVM，针对小型设备的Go编译器</font>

TinyGo是一个将Go语言带入具有单处理器内核的微控制器和小型系统的项目，其通过创建基于LLVM的新编译器来实现在微控制器上运行Go程序，这有望带来更小更高效的代码，并且肯定会带来更大的灵活性。  

> 项目官网：https://tinygo.org/
> 项目主页：https://github.com/tinygo-org/tinygo

TinyGo目前已支持多达48种不同的板和设备，如Arduino Nano33 IoT、Adafruit Circuit Playground Express、BBC micro:bit等等。

如下是一个非常简单的LED闪烁demo：

```Go
package main

import (
    "machine"
    "time"
)

func main() {
    led := machine.LED
    led.Configure(machine.PinConfig{Mode: machine.PinOutput})
    for {
        led.Low()
        time.Sleep(time.Millisecond * 1000)

        led.High()
        time.Sleep(time.Millisecond * 1000)
    }
}
```

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

