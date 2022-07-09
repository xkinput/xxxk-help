# 项目概述

## 项目背景

**小小星空**是一个致力于将**星空系列汉字编码方案**挂载到**小小输入法**的项目。

对于初学者，你可能需要先了解以下名词：

* **输入法**：一个笼统的概念，可能被用于表示**编码方案**或**输入法编辑器**。
* **汉字编码方案**：将键盘编码映射为汉字的一套规则，例如全拼、王码五笔、小鹤双拼等。本项目主要使用 *@吅吅大山* 创造的星空系列方案，是一类以[顶功上屏](https://zhuanlan.zhihu.com/p/291029476)、易学易用为主要特色的汉字编码方案。
* [输入法编辑器](https://docs.microsoft.com/zh-cn/windows/uwp/design/input/input-method-editors)（input method editor）：接受用户键盘输入，依照某一输入方案进行处理，并输出相应文字符号的软件。常见的有：搜狗拼音输入法、王码五笔输入法、小鹤音形输入法等。其中，有一类特殊的输入法，例如[中州韵输入法引擎](https://rime.im/)（Rime Input Method Engine）、[多多输入法生成器](https://www.chinput.com/portal.php)、[小小输入法][小小论坛]（Yong）等，它们不专精于一种汉字编码方案，而是打造一个能够挂载各种编码方案的通用平台。本项目所使用的输入平台是由 *@dgod* 开发的小小输入法。

> 与本项目类似的项目有：[:fa fa-github: RIME键道][RIME键道仓库]，[:fa fa-github: RIME星空两笔](https://gitee.com/morler/rime_xklb)等。它们的区别主要是小小输入法与RIME输入法的区别（**纯属个人观点，详细的差异还需亲身使用对比方能感知**）：
> * 小小输入法：在 Windows 平台上的安装和使用更加方便和流畅
> * RIME输入法：跨平台更多（支持苹果）、支持 [:fa fa-github: 脚本扩展](https://github.com/tswwe/my-rime-lua)

## 快速上手

### 如果你是普通用户...

若想直接使用本项目的成果，请下载由本项目编译而成的**小小星空输入法**安装包：

* 下载地址1：[:fa fa-github: 小小星空仓库的发行版页面](https://github.com/xkinput/xxxk/releases)
* 下载地址2：[:fa fa-hdd-o: 永硕E盘][小小星空网盘]

下载完成后，别忘了继续阅读本文档。本文档主要包含以下章节，可在左侧边栏中快速定位：

* [方案介绍](schema.md)：新手必读——星空系列方案入门理论课
* [安装小小](install.md)：新手必读——如何安装小小星空输入法
* [使用小小](usage.md)：用户手册——如何使用小小输入法
* [开发指南](develop.md)：开发者手册——如何参与贡献本项目
* [其他资源](res.md)：一些好用的资源、工具和网站
* [更新历史](history.md)：记录项目成长点滴

### 如果你是开发者...

除了阅读本文档，你也可前往 [:fa fa-github: 小小星空仓库][小小星空仓库] 查看本项目的结构。总的来说，本项目对小小输入法的修改被分类组织在不同的一级目录中，如下表所示。

| 目录              | 作用                                                 |
| ----------------- | ---------------------------------------------------- |
| xxxk-xkcommon     | 星空公用包。下面的每个星空系列方案都依赖于该公用包。 |
| xxxk-schema-xkjd6 | 星空键道6方案。                                      |
| xxxk-schema-xklb  | 星空两笔方案。                                       |
| xxxk-schema-xkyb  | 星空一笔方案。                                       |
| xxxk-schema-xkxb  | 星空星笔方案。                                       |

## 致谢

本项目离不开社区中的各位大佬和以下项目的支持：

### 社区

* [:fa fa-qq: 星空QQ群：320053116][星空QQ群] —— 接近满员，建议加入分流的键道QQ群
* [:fa fa-qq: 键道QQ群：865189947][键道QQ群]
* [:fa fa-telegram: 星空电报交流群][星空电报群]

### 项目

* [:fa fa-home: 星空官网][星空官网] —— 星空门户网站
* [:fa fa-home: RIME键道](https://github.com/xkinput/Rime_JD) —— 本项目内置键道方案的码表来源
* [:fa fa-hdd-o: 大牛的网盘](http://daniushuangpin.ysepan.com) —— 本项目内置星空一笔、星空二笔、星空星笔方案的码表来源
* [:fa fa-home: 字海两分输入法](http://cheonhyeong.com/Simplified/download.html) —— 本项目内置字海两分方案的码表来源
* [:fa fa-home: 小小输入法][小小输入法论坛] —— 本项目所用的输入法平台

[星空QQ群]: https://jq.qq.com/?_wv=1027&k=5tVcZlL
[键道QQ群]: https://jq.qq.com/?_wv=1027&k=WxhhXU6u
[星空电报群]: https://t.me/xkinput

[星空官网]: https://xkinput.github.io
[RIME键道文档]: https://pingshunhuangalex.gitbook.io/rime-xkjd
[RIME键道仓库]: https://github.com/xkinput/Rime_JD

[小小星空首页]: https://xkinput.github.io/xxxk-help
[小小星空仓库]: https://github.com/xkinput/xxxk
[小小星空网盘]: http://xxxk.ysepan.com/

[小小输入法网盘]: http://yongim.ysepan.com
[小小输入法论坛]:http://yong.dgod.net
[小小输入法仓库]: https://github.com/dgod/yong
