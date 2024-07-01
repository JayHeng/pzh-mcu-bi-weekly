# 痞子衡嵌入式半月刊： 第 103 期

![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 102 期》](https://www.cnblogs.com/henjay724/p/18266049)

## 唠两句

历史上的今天：

本期共 3 个项目，希望对你有帮助！

## 项目类

### <font color="red">1、tslib - 嵌入式中使用最广泛的电阻触摸屏校正算法库</font>

tslib 是嵌入式系统里用得最多的触摸屏校正算法库，其充分利用了矩阵的平移，旋转和缩放等运算。tslib 常用于对电阻触摸屏的功能调试，能够为触摸屏驱动获得的采样提供诸如滤波、去抖、校准等功能，通常作为触摸屏驱动的适配层，为上层的应用提供了一个统一的接口。

 * 项目地址：https://github.com/libts/tslib

### <font color="red">2、cotParam - 基于C语言的轻量级参数管理框架</font>

cotParam 是一个参数管理框架代码，其功能就是统一管理软件中的各类系统数据参数。该参数管理并不涉及数据是如何储存的。因为有些系统数据并不需要储存起来，只需要进行管理而已。

 * 项目地址：https://gitee.com/cot_package/cot_param

cotParam 主要特点有：

```text
1. 采用表驱动方式统一管理所有参数，包括缺省值、最小值和最大值等
2. 采用宏定义快速注册和添加参数进行管理
3. 支持基本类型参数和字符串参数
4. 支持序列化和反序列化，便于保存和读取校验
5. 可通过串口协议或其他协议调用接口修改参数
```

 ### <font color="red">3、cotMenu - 轻量级多级菜单控制框架程序</font>

cotMenu 是一个降低了耦合性，完全独立的菜单框架，菜单显示风格和显示平台完全由自己根据需求设计，而菜单操作统一由菜单模块处理即可，提高程序的移植性。

 * 项目地址：https://gitee.com/cot_package/cot_menu

cotMenu 主要特点有：

```text
1. 采用链表方式实现多级菜单（通过配置选择采用动态分配或者数组实现）
2. 菜单框架作为独立模块，拒绝和按键模块、显示模块进行耦合
3. 在十分独立的情况下，也保证不受菜单的显示风格和显示平台影响，可自由选择设计显示风格和显示平台
4. 快捷菜单操作等
5. 可以采用表驱动的方式初始化菜单，提高代码的可读性
```

 ![](https://raw.githubusercontent.com/JayHeng/pzh-mcu-bi-weekly/master/pics/issue-103/.PNG)

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](https://raw.githubusercontent.com/JayHeng/pzhmcu-picture/master/wechat/pzhMcu_qrcode_258x258.jpg)

