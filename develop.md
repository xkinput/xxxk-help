# :fa fa-code-fork: 开发指南

前往 [:fa fa-github: 本项目仓库][小小星空仓库]获取源代码。解压后可以得到三个一级目录：

* `📂build`：存放编译生成**小小星空输入法**安装包的脚本。
* `📂data`：编译**小小星空输入法**安装包所需的程序文件。具体的程序文件不在本仓库中，需要由原版小小输入法的安装包解包得到，详见下面的说明。
* `📂home`：各种魔改原版**小小输入法**的数据文件，以及星空系列方案的码表文件。

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
[RIME键道文档]: https://pingshunhuangalex.gitbook.io/rime-xkjd
[RIME键道仓库]: https://github.com/xkinput/Rime_JD

[小小星空首页]: https://xkinput.github.io/xxxk-help
[小小星空仓库]: https://github.com/xkinput/xxxk
[小小星空网盘]: http://xxxk.ysepan.com

[小小输入法网盘]: http://yongim.ysepan.com
[小小输入法论坛]: https://yong.dgod.net
[小小输入法仓库]: https://github.com/dgod/yong