# :fa fa-code-fork: 开发指南

前往 [:fa fa-github: 本项目仓库][小小星空仓库]获取源代码。解压后可以得到三个一级目录：

* `📂build`：存放编译生成**小小星空输入法**安装包的脚本。
* `📂data`：编译生成**小小星空输入法**安装包所需的程序文件，通常由原版小小输入法安装包解包而得。
* `📂home`：各种魔改原版**小小输入法**的数据文件，以及星空系列方案的码表文件。

?> 本项目依赖的小小输入法正在逐步开源，其 Linux 版本已全部开源，详见[:fa fa-github: 小小输入法项目仓库][小小输入法仓库]。

按照以下步骤，即可将本项目编译生成小小星空输入法安装包：

<!-- tabs:start -->

### ** Windows **

1. 把原版**小小输入法**的程序目录 `yong` 里的内容放到 `data/yong-win` 目录下。
2. 部署 NSIS，编译 `build/win/xxxk.nsi`。

### ** Android **

1. 下载[原版小小输入法 Android 版安装程序](http://yong.dgod.net/sync/yong-android/yong.apk)，把 yong.apk 放到 `data/yong-android` 目录下。
2. 下载 [apktool](https://apktool.org/docs/install)，把 apktool.jar 和 apktool.bat 放到 `data/yong-android` 目录下。
3. 下载 [uber-apk-signer](https://github.com/patrickfav/uber-apk-signer)，把 uber-apk-signer.jar 放到 `data/yong-android` 目录下。
4. 运行 xxxk.bat，执行 [A] 选项，得到 xxxk-signed.apk。

?> 以上编译工具依赖 java8 或更高版本。

### ** Linux **

请转至[:fa fa-github: 小小输入法项目仓库][小小输入法仓库]获取原版小小输入法 Linux 版的源代码。

<!-- tabs:end -->

在编译之前，您也可以先对项目进行修改：

* 定制 Windows 版编译脚本：待补充
* [定制皮肤（PC）](develop-skin-pc.md)
* 定制皮肤（Android）：待补充

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

