# 痞子衡嵌入式半月刊： 第 47 期

![](http://henjay724.com/image/cnblogs/pzh_mcu_bi_weekly.PNG)

这里分享嵌入式领域有用有趣的项目/工具以及一些热点新闻，农历年分二十四节气，希望在每个交节之日准时发布一期。

本期刊是开源项目（GitHub: [JayHeng/pzh-mcu-bi-weekly](https://github.com/JayHeng/pzh-mcu-bi-weekly)），欢迎提交 issue，投稿或推荐你知道的嵌入式那些事儿。

**上期回顾** ：[《痞子衡嵌入式半月刊： 第 46 期》](https://www.cnblogs.com/henjay724/p/15706368.html)

## 唠两句

本周三是小寒，历史上的今天：2007年1月9日，备受瞩目的A股保险第一股 — 中国人寿（601628）于在上海证券交易所挂牌上市。

本期共收录 0个资讯、1个项目、3个工具，希望对你有帮助！

## 资讯类

## 项目类

### <font color="red">1、advent-calendar-of-circuits-2020 - 一个月每天用KiCad设计一个PCB项目</font>

Gregory Davill 是来自澳大利亚的一个技术牛人，在开源硬件领域非常有名且活跃。他在2020年12月坚持每一天设计一个电路板，用 KiCad 完成电路设计到 PCB 的布局布线完成，这便是 advent-calendar-of-circuits-2020 项目。

> * 项目地址：https://github.com/gregdavill/advent-calendar-of-circuits-2020

电子森林苏老师将这 31 个项目全部整理了出来，这对于正在学习、使用 KiCad 的工程师朋友一定很有帮助。

> * 全部项目：https://www.eetree.cn/doc/detail/2330

![](http://henjay724.com/image/biweekly20220109/advent-calendar-of-circuits-2020.PNG)

## 工具类

### <font color="red">1、gcov - 标准c/c++代码覆盖率测试工具</font>

gcov 全称 GCC Coverage，是一个测试代码覆盖率的工具，命令行方式的控制台程序，伴随GCC发布，配合GCC共同实现对C/C++文件的语句覆盖和分支覆盖测试；

> * 工具地址：https://gcc.gnu.org/onlinedocs/gcc/Gcov.html

gcov 可以统计每一行代码的执行频率，实际上哪些代码确实被执行了，每一段代码(section code)的耗时(执行时间)，因此，gcov可以帮你优化代码，当然这个优化动作还是应该由开发者完成。

![](http://henjay724.com/image/biweekly20220109/gcov.PNG)

### <font color="red">2、lcov - GCC测试覆盖率的前端图形展示工具</font>

lcov 是 GCC 测试覆盖率的前端图形展示工具，简单说就是 gcov 结果展现的一个前端。它通过收集多个源文件的行、函数和分支的代码覆盖信息（程序执行之后生成gcda、gcno文件） 并且将收集后的信息生成 HTML 页面。

> * 结果示例：http://ltp.sourceforge.net/coverage/lcov/output/index.html

![](http://henjay724.com/image/biweekly20220109/lcov.PNG)

### <font color="red">3、gprof - 标准c/c++代码性能分析工具</font>

gprof 全称 GNU profiler，是一个性能分析工具。gprof 可以显示程序运行的“flat profile”，包括每个函数的调用次数，每个函数消耗的处理器时间。也可以显示“调用图”，包括函数的调用关系，每个函数调用花费了多少时间。还可以显示“注释的源代码”，是程序源代码的一个复本，标记有程序中每行代码的执行次数。

> * 工具说明：http://sourceware.org/binutils/docs/gprof/

### 欢迎订阅

文章会同时发布到我的 [博客园主页](https://www.cnblogs.com/henjay724/)、[CSDN主页](https://blog.csdn.net/henjay724)、[知乎主页](https://www.zhihu.com/people/henjay724)、[微信公众号](http://weixin.sogou.com/weixin?type=1&query=痞子衡嵌入式) 平台上。

微信搜索"__痞子衡嵌入式__"或者扫描下面二维码，就可以在手机上第一时间看了哦。

![](http://henjay724.com/image/github/pzhMcu_qrcode_258x258.jpg)

