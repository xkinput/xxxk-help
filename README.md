# 小小星空

《小小星空》是一个致力于将星空系列汉字编码方案挂载到小小输入法的项目。本项目的主页是：[xkinput.github.io/xxxk-help](https://xkinput.github.io/xxxk-help)。

## 项目简介

* **输入法**：一个笼统的概念，可能被用于表示**编码方案**或**输入法编辑器**。
* **汉字编码方案**：将键盘编码映射为汉字的一套规则，例如全拼、王码五笔、小鹤双拼等。本项目主要使用*吅吅大山*创造的星空系列方案，是一类以[顶功上屏 :fa fa-external-link:](https://zhuanlan.zhihu.com/p/291029476)、易学易用为主要特色的汉字编码方案。
* [输入法编辑器 :fa fa-external-link:](https://docs.microsoft.com/zh-cn/windows/uwp/design/input/input-method-editors)（input method editor）：接受用户键盘输入，依照某一输入方案进行处理，并输出为相应文字符号的软件。常见的输入法有：搜狗拼音输入法、王码五笔输入法、小鹤音形输入法等。其中，有一类特殊的输入法，例如[中州韵输入法引擎 :fa fa-external-link:](https://rime.im/)（Rime Input Method Engine）、[多多输入法生成器 :fa fa-external-link:](https://www.chinput.com/portal.php)、[小小输入法 :fa fa-external-link:](http://yong.dgod.net/)（Yong）等，它们不专精于一种汉字编码方案，而是打造一个能够挂载各种编码方案的通用平台。本项目所使用的输入平台是由*dgod*开发的小小输入法 ，其Windows版本在部署方便、运行流畅、功能丰富等方面获得了极佳的平衡。
* **小小星空**：即本项目，致力于将星空系列汉字编码方案挂载到小小输入法上，并进行适当的优化。本项目对小小输入法的修改被分类组织在不同的一级目录中，如下表所示。经过本项目扩展的小小输入法，称为**小小星空输入法**。

| 目录              | 作用                                                 |
| ----------------- | ---------------------------------------------------- |
| xxxk-xkcommon     | 星空公用包。下面的每个星空系列方案都依赖于该公用包。 |
| xxxk-schema-xkjd6 | 星空键道6方案。                                      |
| xxxk-schema-xklb  | 星空两笔方案。                                       |
| xxxk-schema-xkyb  | 星空一笔方案。                                       |
| xxxk-schema-xkxb  | 星空星笔方案。                                       |

