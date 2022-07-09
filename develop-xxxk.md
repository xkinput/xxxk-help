# 定制本项目

## 复刻源码

前往 [:fa fa-github: 项目仓库][小小星空仓库]，获取本项目源码。

## 项目架构

如[快速上手](/README#如果你是开发者)章节所述，本项目主要包含以下内容：

### xxxk-xkcommon目录

包含对小小输入法的一系列功能增强。包括但不限于：

* 全拼输入方案（`xxxk-xkcommon\entry`，`xxxk-xkcommon\mb\pinyin`）：一个备用的本地全拼输入方案。按 <kbd>u</kbd> 可开启笔画模式。
* 星空扩展码表（`xxxk-xkcommon\mb\*.txt`）：适合星空方案使用的一些扩展码表，例如 <kbd>o</kbd> 引导的特殊符号或命令、<kbd>;</kbd> 引导的特殊符号等。
* 增强的英文词库（`xxxk-xkcommon\mb\english.txt`）：来自 [Github](https://github.com/dwyl/english-words) 的英文单词词库，比原版收词更多。
* 脚本（`xxxk-xkcommon\tools`）：一些 bat 和 vbs 脚本，可被码表调用，实现某些特殊任务。
* 中文标点映射（`xxxk-xkcommon\bd.txt`）：实现按 <kbd>/</kbd> 键输出 `、` 等功能。
* 增强的笔画库（`xxxk-xkcommon\bihua.bin`）：可供其他方案的笔画模式调用。数据来自 2018 年的汉典，比小小输入法原版内置的数据库收字更多。
* 火星文之菊花文（`xxxk-xkcommon\crab.txt`）：<kbd>Ctrl</kbd><kbd>Alt</kbd><kbd>Shift</kbd><kbd>H</kbd> 开启，开启后输出的文字带有菊花特效。（小小星空已默认配置好，其他基于小小输入法的项目若想使用，需确保 `yong.ini` 中设置 `crab=crab.txt`，并在 `[key]crab` 设置开启热键）
* 增强的软键盘（`xxxk-xkcommon\keyboard.ini`）：参考[小小论坛@qwer的帖子](http://yong.dgod.net/read.php?tid=3479)，对软键盘进行强化。
* 键位映射（`xxxk-xkcommon\layout.txt`）：仅仅写了一个配置文件模板，供感兴趣者参考，在此基础上修改，可以实现键位映射、并击等高级功能。默认未开启。（如要开启，需在 `yong.ini` 中设置 `[IM]layout=layout.txt`）
* 定制菜单（`xxxk-xkcommon\menu.ini`）：小小星空定制的输入法右键菜单。（小小星空已默认配置好，其他基于小小输入法的项目若要调用，可在 `yong.ini` 中设置 `[IM]menu=menu.ini`）
* 网址屏蔽配置（`xxxk-xkcommon\urls.txt`）：小小输入法默认会自动识别 `http`、`ftp` 等开头的编码并转入英文模式，可能会干扰一些中文输入方案的使用。该文件可以屏蔽这个功能。
* 懒人的输入法配置（`xxxk-xkcommon\yong.ini`）：输入法配置文件，定制了输入法的外观、热键、某些行为等。可以直接使用，也可以在此基础上，参考 `yong.chm` 进行个性化定制。
* 编译脚本（`yong_thxnder_gb18030.nsi`）：NSIS 脚本文件，可以编译生成小小星空输入法安装包。已经添加了详细的注释，可供参考。

### xxxk-schema-xkjd6目录

用于小小输入法的星空键道6方案。包括：

* 本地文档（`xxxk-schema-xkjd6\doc`）：提取自多多输入法的文档，主要介绍了键道6方案。
* 星空键道6输入方案（`xxxk-schema-xkjd6\entry`，`xxxk-schema-xkjd6\mb`）：方案的入口文件、码表文件等。
* 键盘图（`xxxk-schema-xkjd6\skin`）

### 其他目录

其他目录结构类似于`xxxk-schema-xkjd6`，不赘述。

## 编译项目

<!-- tabs:start -->

### ** Windows **

1. 下载[原版小小输入法 Windows 版][小小输入法网盘]（7z格式）并解压。
2. 将本项目的各个一级目录（如 `xxxk-xkcommon`）下的文件依次复制粘贴到解压后的程序目录下。
3. 根据自己的需要，修改 `xxxk-xkcommon/yong_thxnder.nsi` 并用 NSIS 2.5 编译生成安装包。编译工具可在[小小星空网盘][小小星空网盘]获取。

### ** Android **

1. 下载[原版小小输入法 Android 版安装程序][小小输入法网盘]，并用 apktool 反编译。
2. 根据自己的需要，修改反编译后的资源文件。例如：
   * `res/drawable-hdpi|mdpi|xhdpi/app_icon.png` 是程序图标，可替换。
   * `assets/mb` 是码表，会被安装到`sdcard/yong/mb`。注意，安卓版不会覆盖安装。
   * `assets/www` 是默认皮肤，一般包括 `fonts` 目录和 `keyboard.css`、`keyboard.html`，不会体现在程序目录中。如果安装完成后想换皮肤，要把皮肤放到 `.yong/android` 目录。
   * `assets/yong.ini` 是初始配置文件。注意，小小安卓版不支持 entry。
3. 用 apktool 重新编译为安装包，并用 autosign 等工具进行签名。

### ** Linux **

请转至[小小输入法的项目仓库][小小输入法仓库]取原版小小输入法 Linux 版的源代码。

<!-- tabs:end -->


[星空QQ群]: https://jq.qq.com/?_wv=1027&k=5tVcZlL
[键道QQ群]: https://jq.qq.com/?_wv=1027&k=WxhhXU6u
[星空电报群]: https://t.me/xkinput

[星空官网]: https://xkinput.github.io
[RIME键道文档]: https://pingshunhuangalex.gitbook.io/rime-xkjd
[RIME键道仓库]: https://github.com/xkinput/Rime_JD

[小小星空首页]: https://xkinput.github.io/xxxk-help
[小小星空仓库]: https://github.com/xkinput/xxxk
[小小星空网盘]: http://xxxk.ysepan.com

[小小输入法网盘]: http://yongim.ysepan.com
[小小输入法论坛]:http://yong.dgod.net
[小小输入法仓库]: https://github.com/dgod/yong

