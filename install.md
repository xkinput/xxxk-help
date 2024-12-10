# :fa fa-download: 安装小小

小小星空输入法是小小输入法的一个再发行版本，理论上和小小输入法一样支持 Windows、Android、Linux 平台，但目前只在 Windows（XP+）和 Android 平台上测试过。

<!-- tabs:start -->

## ** Windows **

### 安装

方式一（自动安装）：如果懒得折腾，可以直接下载并运行打包好的[小小星空输入法 Windows 版安装程序][小小星空网盘]。这种方式不兼容系统上已经安装的小小输入法。

方式二（手动安装）：已经安装了[原版小小输入法 Windows 版][小小输入法网盘]的用户，可以从[:fa fa-github: 小小星空仓库][小小星空仓库]下载本项目源代码，然后将 `home` 目录里的内容（最关键的是 `mb` 和 `entry` 目录）复制到小小输入法的配置目录中，然后将 yong-win.ini 更名为 yong.ini。

### 启动

安装成功后，系统设置里会多出一个 Yong 输入法键盘。

![系统语言和键盘](_media\lang-and-kbd-win10.png 'Win10：语言 🞂 中文语言选项 🞂 键盘')

![系统语言和键盘](_media\lang-and-kbd-win7.png 'Win7：区域和语言 🞂 键盘和语言 🞂 更改键盘')

![系统语言和键盘](_media\lang-and-kbd-xp.png 'XP：区域和语言选项 🞂 语言 🞂 详细信息；还要勾选“将高级文字服务支持应用于所有程序”；SP2 以下还需安装 wic 组件')

!> 如果 TSF 模块没有成功安装，则不会多出 Yong 输入法键盘，输入法将无法以 TSF 模式启动，但是可以以外挂模式启动（此模式不支持光标跟随）。

第一步（如果想要以外挂模式启动，请跳过此步）：把光标定位到任意文本框，然后如图在任务栏托盘或语言工具栏中切换到 Yong 输入法键盘（也可以用快捷键切换，一般是<kbd>Ctrl</kbd><kbd>Shift</kbd>或<kbd>Win</kbd><kbd>Space</kbd>）。如果系统只有 Yong 输入法一个键盘，则不需要切换键盘，此步跳过。

![切换系统键盘](_media\run-tsf-on-win10.png 'Win10')
![切换系统键盘](_media\run-tsf-on-win7.png 'Win7')
![切换系统键盘](_media\run-tsf-on-xp.png 'XP')

第二步：从开始菜单启动输入法主程序。

第三步（Win7 以下不需要此步）：把光标定位到任意文本框，然后使用<kbd>Ctrl</kbd><kbd>Space</kbd>快捷键，呼出小小输入法的状态条。（如果成功安装了 TSF 模块，Win8 以上系统也可以鼠标点击任务栏托盘的「英」，Win7 以下系统可以鼠标点亮任务栏托盘的小小输入法图标，来呼出小小输入法的状态条）

?> 判断输入法运行在 TSF 模式还是外挂模式的方法：右击输入法状态条，如果看到“TSF 模式未生效”的菜单项，说明正以外挂模式运行，否则以 TSF 模式运行。

### 退出 · 重启 · 重载

这些命令都包含在输入法状态条的右键菜单中。

?> **重载**即重新载入配置，而不需要**重启**输入法。码表文件和部分配置项只需要重载就可以生效。鼠标中键单击输入法状态条也可以重载。

### 卸载

从开始菜单、控制面板或者程序目录执行卸载程序即可。

?> 由于 Win10 的一个[疑似 bug](https://answers.microsoft.com/zh-hans/windows/forum/all/%E7%A8%8B%E5%BA%8F%E7%9A%84%E5%8D%B8%E8%BD%BD/0b57356b-e988-486e-b863-1cf63e0cf0d2)，开始菜单中可能无法显示卸载程序。

## ** Android **

### 安装

方式一（自动安装；仅供测试，更推荐方式二）：直接使用打包好的[小小星空输入法 Android 版安装程序][小小星空网盘]。

!> 目前的安装包无法自动删除 `sdcard/yong/.yong` 目录，建议安装之前先手动删除 `sdcard/yong/.yong/yong.ini`。

方式二（手动安装）：如果手机上已经安装了[原版小小输入法 Android 版][小小输入法网盘]，可以从[:fa fa-github: 小小星空仓库][小小星空仓库]下载本项目源代码，将 `home` 目录里的内容（最关键的是 `mb` 目录）复制到 `sdcard/yong/.yong` 中，然后将 yong-android.ini 更名为 yong.ini。

### 启动

1. 运行 Yong 输入法图形设置程序，授予必须的权限（必须授予的权限有：“允许应用显示悬浮窗”，“允许访问所有文件”，建议授予的权限有：“自启动”、“读取通知类短信”、“读取联系人”、“读写剪切板”等）。
2. 在**图形设置界面 🞂 安卓 🞂 设置系统输入法**（或者在手机的**设置 🞂 更多设置 🞂 语言与输入法设置 🞂 输入法管理**中），启用 Yong 输入法。
3. 在任意地方呼出输入法键盘，并切换当前输入法为 Yong 输入法（如果无法切换，在手机的**设置 🞂 更多设置 🞂 语言与输入法设置 🞂 当前输入法管理**中，选择 Yong 输入法）。如果顺利的话，你将看到Yong输入法的键盘，并且手机里会生成 `sdcard/yong/.yong` 目录（这是一个隐藏目录，系统自带的文件管理器可能看不到）。

### 退出

在手机的**设置 🞂 应用设置 🞂 应用管理**中结束 Yong 输入法。

## ** Linux **

!> 该安装方式尚未测试，不一定适用于所有Linux发行版。

### 安装

1. 下载并解压[原版小小输入法 Linux 版][小小输入法网盘]（形如 `yong-lin-xxx.7z`）得到 `yong` 程序目录（可以覆盖已安装的旧版程序目录）。
2. 从[:fa fa-github: 小小星空仓库][小小星空仓库]下载本项目源代码，将 `home` 目录里的内容（最关键的是 `mb` 和 `entry` 目录）复制到小小输入法的配置目录中，然后将 yong-win.ini 更名为 yong.ini。
3. 在终端中进入程序目录，并执行命令 `sudo ./yong-tool.sh --install`。如果想作为默认输入法，接着执行 `./yong-tool.sh --select`。

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