# 项目概述

**小小星空**是一个致力于将**星空系列汉字编码方案**挂载到**小小输入法**的项目。

> 与本项目类似的项目有：[:fa fa-home: RIME键道](https://github.com/xkinput/Rime_JD)。二者的区别主要是小小输入法与RIME输入法的区别：
> * 小小输入法：在Windows平台上的安装和使用更加方便和流畅
> * RIME输入法：跨平台更多（支持苹果）、可编写脚本扩展（例如[:fa fa-github: 我的RIME脚本仓库](https://github.com/tswwe/my-rime-lua)）
>
> （以上纯属个人观点，详细的差异还需亲身使用对比方能感知）

## 名词解释

* **输入法**：一个笼统的概念，可能被用于表示**编码方案**或**输入法编辑器**。
* **汉字编码方案**：将键盘编码映射为汉字的一套规则，例如全拼、王码五笔、小鹤双拼等。本项目主要使用*吅吅大山*创造的星空系列方案，是一类以[顶功上屏](https://zhuanlan.zhihu.com/p/291029476)、易学易用为主要特色的汉字编码方案。
* [输入法编辑器](https://docs.microsoft.com/zh-cn/windows/uwp/design/input/input-method-editors)（input method editor）：接受用户键盘输入，依照某一输入方案进行处理，并输出相应文字符号的软件。常见的有：搜狗拼音输入法、王码五笔输入法、小鹤音形输入法等。其中，有一类特殊的输入法，例如[中州韵输入法引擎](https://rime.im/)（Rime Input Method Engine）、[多多输入法生成器](https://www.chinput.com/portal.php)、[小小输入法](http://yong.dgod.net/)（Yong）等，它们不专精于一种汉字编码方案，而是打造一个能够挂载各种编码方案的通用平台。本项目所使用的输入平台是由*dgod*开发的小小输入法 ，其Windows版本在部署方便、运行流畅、功能丰富等方面获得了极佳的平衡。

## 快速上手

本项目基于**小小输入法**进行了一些定制，以使其能更好地使用**星空系列汉字编码方案**。

### 如果你是普通用户...

若想直接使用本项目的成果，请下载由本项目编译而成的**小小星空输入法**安装包：

* 下载地址1：[:fa fa-github: 项目仓库的发行版页面](https://github.com/xkinput/xxxk/releases)
* 下载地址2：[:fa fa-hdd-o: 永硕E盘](http://xxxk.ys168.com)

下载完成后，别忘了阅读本文档↓↓↓

### 本文档的食用方法

在使用过程中有任何疑问，可以查阅本文档。本文档主要包含以下章节，可在左侧边栏中快速定位：
* [方案介绍](schema.md)：新手必读——星空系列方案入门理论课
* [安装小小](install.md)：新手必读——如何安装小小星空输入法
* [使用小小](usage.md)：用户手册——如何使用小小输入法
* [开发指南](develop.md)：开发者手册——如何参与贡献本项目
* [其他资源](res.md)：一些好用的资源、工具和网站
* [社区支持](community.md)：加入星空大家庭，一起讨论和学习
* [更新历史](history.md)：记录项目成长点滴

### 如果你是开发者...

可前往[:fa fa-github: 项目仓库](https://github.com/xkinput/xxxk) 查看本项目的结构。总的来说，本项目对小小输入法的修改被分类组织在不同的一级目录中，如下表所示。

| 目录              | 作用                                                 |
| ----------------- | ---------------------------------------------------- |
| xxxk-xkcommon     | 星空公用包。下面的每个星空系列方案都依赖于该公用包。 |
| xxxk-schema-xkjd6 | 星空键道6方案。                                      |
| xxxk-schema-xklb  | 星空两笔方案。                                       |
| xxxk-schema-xkyb  | 星空一笔方案。                                       |
| xxxk-schema-xkxb  | 星空星笔方案。                                       |

