# :fa fa-code-fork: 开发指南

前往 [:fa fa-github: 本项目仓库][小小星空仓库]获取源代码。解压后可以得到三个一级目录：

* `📂app-win`：存放编译生成**小小星空输入法**安装包的脚本。
* `📂data-base`：对原版**小小输入法**的一部分配置文件进行魔改得到的文件。
* `📂data-schema`：**星空系列方案**的核心文件。

?> 本项目依赖的小小输入法正在逐步开源，其 Linux 版本已全部开源，详见[:fa fa-github: 小小输入法项目仓库][小小输入法仓库]。

按照以下步骤，即可将本项目编译生成小小星空输入法安装包：

<!-- tabs:start -->

### ** Windows **

1. 把原版**小小输入法**的程序目录 `yong` 放到 `app-win` 目录下。
2. 根据自己的需要，修改 `app-win`、`data-base` 和 `data-schema` 目录下的文件。
3. 安装 NSIS，编译 `app-win/nsis/xxxk.nsi`。

### ** Android **

1. 下载[原版小小输入法 Android 版安装程序][小小输入法网盘]，并用 apktool 反编译。
2. 根据自己的需要，修改反编译后的资源文件。例如：
   * `res/drawable-hdpi|mdpi|xhdpi/app_icon.png` 是程序图标，可替换。
   * `assets/mb` 是码表，会被安装到`sdcard/yong/mb`。注意，安卓版不会覆盖安装。
   * `assets/www` 是默认皮肤，一般包括 `fonts` 目录和 `keyboard.css`、`keyboard.html`，不会体现在程序目录中。如果安装完成后想换皮肤，要把皮肤放到 `.yong/android` 目录。
   * `assets/yong.ini` 是初始配置文件。注意，小小安卓版不支持 entry。
3. 用 apktool 重新编译为安装包，并用 autosign 等工具进行签名。

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

