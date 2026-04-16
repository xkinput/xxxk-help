# :fa fa-code-fork: 开发指南

前往 [:fa fa-github: 本项目仓库][小小星空仓库]获取源代码。解压后可以得到三个一级目录：

* `📂build`：存放编译生成**小小星空输入法**安装包的脚本。
* `📂data`：编译**小小星空输入法**安装包所需的程序文件。具体的程序文件不在本仓库中，需要由原版小小输入法的安装包解包得到，详见下面的说明。
* `📂home`：各种魔改原版**小小输入法**的数据文件，以及星空系列方案的码表文件。包括但不限于：

  * 全拼输入方案（`home/entry`，`home/mb/pinyin`）：一个备用的本地全拼输入方案。按 <kbd>u</kbd> 可开启笔画模式。
  * 星空扩展码表（`home/mb`）：适合星空方案使用的一些扩展码表，例如 <kbd>o</kbd> 引导的特殊符号或命令、<kbd>;</kbd> 引导的特殊符号等。
  * 增强的英文词库（`home/mb/english.txt`）：来自 [Github](https://github.com/dwyl/english-words) 的英文单词词库，比原版收词更多。
  * 脚本（`home/tools`）：一些 bat 和 vbs 脚本，可被码表调用，实现某些特殊任务。
  * 中文标点映射（`home/bd.txt`）：实现按 <kbd>/</kbd> 键输出 `、` 等功能。
  * 增强的笔画库（`home/bihua.bin`）：可供其他方案的笔画模式调用。数据来自 2018 年的汉典，比小小输入法原版内置的数据库收字更多。
  * 火星文之菊花文（`home/crab.txt`）：<kbd>Ctrl</kbd><kbd>Alt</kbd><kbd>Shift</kbd><kbd>H</kbd> 开启，开启后输出的文字带有菊花特效。（小小星空已默认配置好，其他基于小小输入法的项目若想使用，需确保 `yong.ini` 中设置 `crab=crab.txt`，并在 `[key]crab` 设置开启热键）
  * ~~增强的软键盘（`home/keyboard.ini`）：参考[小小论坛@qwer的帖子](http://yong.dgod.net/read.php?tid=3479)，对软键盘进行强化。~~
  * ~~键位映射（`home/layout.txt`）：仅仅写了一个配置文件模板，供感兴趣者参考，在此基础上修改，可以实现键位映射、并击等高级功能。默认未开启。（如要开启，需在 `yong.ini` 中设置 `[IM]layout=layout.txt`）~~
  * 定制菜单（`home/menu.ini`）：小小星空定制的输入法右键菜单。（小小星空已默认配置好，其他基于小小输入法的项目若要调用，可在 `yong.ini` 中设置 `[IM]menu=menu.ini`）
  * 网址屏蔽配置（`home/urls.txt`）：小小输入法默认会自动识别 `http`、`ftp` 等开头的编码并转入英文模式，可能会干扰一些中文输入方案的使用。该文件可以屏蔽这个功能。
  * 懒人的输入法配置（`home/yong-win.ini` 和 `home/yong-android.ini`）：输入法配置文件，定制了输入法的外观、热键、某些行为等。可以直接使用，也可以在此基础上，参考 `yong.chm` 进行个性化定制。
  * 编译脚本（`yong_thxnder_gb18030.nsi`）：NSIS 脚本文件，可以编译生成小小星空输入法安装包。已经添加了详细的注释，可供参考。

按照以下步骤，即可将本项目编译生成 Windows 或 Android 版小小星空输入法安装包：

<!-- tabs:start -->

### ** Windows **

1. 部署 [NSIS](https://nsis.sourceforge.io/Download)，下载依赖文件 [EnumINI.nsh](https://nsis.sourceforge.io/Enumerate_INI) 到 NSIS 程序目录/Include 目录下。
2. 下载[原版小小输入法 Windows 版压缩包][小小输入法网盘]（如 yong-win-3.0.0.1.7z）并解压，将 yong 目录中的内容放到本仓库的 data/yong-win 目录下。
3. 执行本仓库的 data/yong-win/yong-update.bat，更新小小输入法程序文件。
4. 用 NSIS 编译本仓库的 build/win/xxxk.nsi 文件，即可得到小小星空的安装包。

### ** Android **

1. 部署 [jdk8](https://openjdk.org) 或更高版本。
2. 下载 [apktool](https://apktool.org/docs/install)，把 apktool.jar 和 apktool.bat 放到本仓库的 data/yong-android 目录下。
3. 下载 [uber-apk-signer](https://github.com/patrickfav/uber-apk-signer)，把 uber-apk-signer.jar 放到本仓库的 data/yong-android 目录下。
4. 下载[原版小小输入法 Android 版安装程序](http://yong.dgod.net/sync/yong-android/yong.apk)，把 yong.apk 放到本仓库的 data/yong-android 目录下。
5. 运行本仓库的 data/yong-android/xxxk.bat，执行 [A] 选项，即可得到小小星空的安装包 xxxk-signed.apk。

### ** Linux **

本项目暂不对 Linux 系统打包制作小小星空的自动安装包。

你可以前往[:fa fa-github: 小小输入法项目仓库][小小输入法仓库]获取原版小小输入法 Linux 版的源代码。

<!-- tabs:end -->

[星空QQ群]: https://jq.qq.com/?_wv=1027&k=5tVcZlL
[键道QQ群]: https://jq.qq.com/?_wv=1027&k=WxhhXU6u
[星空电报群]: https://t.me/xkinput

[星空官网]: https://xkinput.github.io
[RIME键道文档]: https://keytao-docs.vercel.app
[RIME键道仓库]: https://github.com/xkinput/KeyTao

[小小星空首页]: https://xkinput.github.io/xxxk-help
[小小星空仓库]: https://github.com/xkinput/xxxk
[小小星空网盘]: http://xxxk.ysepan.com

[小小输入法网盘]: http://yongim.ysepan.com
[小小输入法论坛]: https://yong.dgod.net
[小小输入法仓库]: https://github.com/dgod/yong