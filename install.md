# :fa fa-download: 安装小小

小小星空输入法是小小输入法的一个再发行版本，理论上和小小输入法一样支持 Windows、Android、Linux 平台，但目前只在 Windows（XP～Win10）和 Android 平台上测试过。

<!-- tabs:start -->

## ** Windows **

### 安装

直接下载并运行打包好的[小小星空输入法 Windows 版安装程序][小小星空网盘]。

?> 已经安装了[原版小小输入法 Windows 版][小小输入法网盘]的用户，也可以手动安装小小星空：从[:fa fa-github: 小小星空仓库][小小星空仓库]下载本项目源代码，将 `data-base` 目录下的文件覆盖到小小输入法的程序目录下，然后将 `data-schema/xkjd6`、`data-schema/xklb` 等目录下的文件依次覆盖到小小输入法的程序目录下。

### 启动

安装成功后，系统设置里会多出一个 Yong 输入法键盘。

![系统语言和键盘](_media\lang-and-kbd-win10.png 'Win10：语言 🞂 中文语言选项 🞂 键盘')

![系统语言和键盘](_media\lang-and-kbd-win7.png 'Win7：区域和语言 🞂 键盘和语言 🞂 更改键盘')

![系统语言和键盘](_media\lang-and-kbd-xp.png 'XP：区域和语言选项 🞂 语言 🞂 详细信息；并且还要勾选“将高级文字服务支持应用于所有程序”')

!> 如果 TSF 模块没有成功安装，则不会多出 Yong 输入法键盘，输入法将无法以 TSF 模式启动，但是可以以外挂模式启动（输入体验较差）。

第一步（如果想要以外挂模式启动，请跳过此步）：把光标定位到任意文本框，然后如图在任务栏托盘或语言工具栏中切换到 Yong 输入法键盘（也可以用快捷键切换，一般是<kbd>Ctrl</kbd><kbd>Shift</kbd>或<kbd>Win</kbd><kbd>Space</kbd>）。如果系统只有 Yong 输入法一个键盘，则不需要切换键盘，此步跳过。

![切换系统键盘](_media\run-tsf-on-win10.png 'Win10')
![切换系统键盘](_media\run-tsf-on-win7.png 'Win7')
![切换系统键盘](_media\run-tsf-on-xp.png 'XP')

第二步：从开始菜单启动输入法主程序（也可以运行程序目录下的`yong.bat`）。

第三步（Win7 以下不需要此步）：把光标定位到任意文本框，然后使用<kbd>Ctrl</kbd><kbd>Space</kbd>快捷键，呼出小小输入法的状态条。（如果成功安装了 TSF 模块，Win8 以上系统也可以鼠标点击任务栏托盘的「英」，Win7 以下系统可以鼠标点亮任务栏托盘的小小输入法图标，来呼出小小输入法的状态条）

?> 判断输入法运行在 TSF 模式还是外挂模式的方法：右击输入法状态条，如果看到“TSF 模式未生效”的菜单项，说明正以外挂模式运行，否则以 TSF 模式运行。

### 退出 · 重启 · 重载 · 重设

这些命令都包含在输入法状态条的右键菜单中。

?> **重载**即重新载入配置，而不需要**重启**输入法。码表文件和部分配置项只需要重载就可以生效。鼠标中键单击输入法状态条也可以重载。

### 卸载

从开始菜单、控制面板或者程序目录执行卸载程序即可。

?> 由于 Win10 的一个[疑似 bug](https://answers.microsoft.com/zh-hans/windows/forum/all/%E7%A8%8B%E5%BA%8F%E7%9A%84%E5%8D%B8%E8%BD%BD/0b57356b-e988-486e-b863-1cf63e0cf0d2)，开始菜单中可能无法显示卸载程序。

## ** Android **

!> 小小输入法安卓版最近更新频繁，本项目尚未跟进，将来更新之后此页面可能发生较大变化。

### 安装

方式一（自动安装）：直接使用打包好的[小小星空输入法 Android 版安装程序][小小星空网盘]。注意，如果手机上已经安装了小小星空输入法或原版小小输入法，需要先卸载它们，并在文件管理器中删除 `sdcard/yong` 目录，然后再进行安装。

!> 目前 Android 版安装程序无法自动删除 `sdcard/yong` 目录下的文件，因此需要用户手动删除该目录。

方式二（手动安装）：如果手机上已经安装了小小星空输入法或者[原版小小输入法 Android 版][小小输入法网盘]，可以采用这种方式。

1. 先退出 Yong 输入法，然后在文件管理器中删除 `sdcard/yong/.yong` 目录（这是个隐藏目录，需要先开启显示隐藏文件）。
2. 将本项目的各个一级目录（如 `xxxk-xkcommon`）下的 `mb` 文件夹依次复制粘贴到 `sdcard/yong` 目录下（如不存在，手动新建）。
3. 将本项目中 `yong_android.ini` 改名为 `yong.ini`，并粘贴到 `sdcard/yong` 目录下。

### 启动

1. 在手机的 <kbd>设置</kbd><kbd>应用设置</kbd><kbd>应用管理</kbd> 中，授予 Yong 输入法足够的权限。必须授予的权限有：“允许应用显示悬浮窗”，建议授予的权限有：“自启动”、“读取通知类短信”、“读取联系人”、“读写剪切板”等。
2. 在手机的 <kbd>设置</kbd><kbd>更多设置</kbd><kbd>语言与输入法设置</kbd><kbd>输入法管理</kbd> 中，启用 Yong 输入法。
3. 在手机的 <kbd>设置</kbd><kbd>更多设置</kbd><kbd>语言与输入法设置</kbd><kbd>当前输入法</kbd> 中，选择 Yong 输入法。
4. 在任意地方呼出输入法键盘。如果顺利的话，你将看到Yong输入法的键盘，并且手机里会生成 `sdcard/yong/.yong` 目录。

### 退出

在手机的 <kbd>设置</kbd><kbd>应用设置</kbd><kbd>应用管理</kbd> 中结束 Yong 输入法。

## ** Linux **

### 安装

1. 下载并解压[原版小小输入法 Linux 版][小小输入法网盘]（形如 `yong-lin-xxx.7z`）得到 `yong` 程序目录（可以覆盖已安装的旧版程序目录）。
2. 下载本项目，并将本项目的各个一级目录（如 `xxxk-xkcommon`）下的文件依次复制粘贴到程序目录下。
3. 在终端中进入程序目录，并执行命令 `sudo ./yong-tool.sh --install`。如果想作为默认输入法，接着执行 `./yong-tool.sh --select`。

!> 该安装方式不一定适用于所有Linux发行版，如果安装遇到问题请自行搜索解决方案。

### 启动

进入系统的区域与语言设置，添加输入法源，选择 <kbd>汉语</kbd><kbd>中文(yong)</kbd>，然后重启。

### 退出

利用小小输入法状态条右键菜单中的退出命令。

### 卸载

在终端中进入程序目录，并执行命令 `sudo ./yong-tool.sh --uninstall`。

<!-- tabs:end -->


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
[小小输入法论坛]: https://yong.dgod.net
[小小输入法仓库]: https://github.com/dgod/yong