# :fa fa-download: 安装小小

小小星空输入法是小小输入法的一个定制版本，和小小输入法一样支持 Windows（XP～Win11）、Android、Linux 系统，不支持 macOS 或 iOS 系统。

<!-- tabs:start -->

## ** Windows **

### 安装

方式一（自动安装）：如果系统里没有已安装的原版小小输入法，可以直接下载并运行打包好的[小小星空输入法 Windows 版安装程序][小小星空网盘]。

> [!THXNOTE|label:执行自动安装时需选择一种安装模式]
> * 标准模式：安装过程会向系统注册 dll 文件，安装完成后输入法以 TSF 模式运行，具有更好的光标跟随能力。
> * 便携模式：安装完成后输入法以外挂模式运行。

方式二（手动安装）：如果系统里已经安装了[原版小小输入法][小小输入法网盘]（并且不打算卸载它），可以先退出原版小小输入法，然后从[:fa fa-github: 小小星空仓库][小小星空仓库]下载本项目源代码，将 home 目录里的内容（最关键的是  mb 和 entry 目录）复制到小小输入法的配置目录中，然后将 yong-win.ini 更名为 yong.ini（删掉原本的 yong.ini）。

> [!TIP|label:小小输入法的配置目录] 
> * 如果小小输入法的程序目录位于 %ProgramFiles% 或 %ProgramFiles(x86)% 目录中，那么配置目录为 %AppData%/yong 目录；
> * 其他情况，配置目录为小小输入法程序目录下的 .yong 目录。

安装完成后，请先确认是否安装了 TSF 模块（即系统设置里是否添加了 Yong 输入法键盘）。如果没有，输入法将只能够以外挂模式运行：

<!-- tabs:start -->

#### ** Win11 **

![系统语言和键盘](_media\lang-and-kbd-win11.webp 'Win11：时间和语言 🞂 语言和区域 🞂 语言选项 🞂 键盘')

#### ** Win10 **

![系统语言和键盘](_media\lang-and-kbd-win10.webp 'Win10：语言 🞂 中文语言选项 🞂 键盘')

#### ** Win7 **

![系统语言和键盘](_media\lang-and-kbd-win7.webp 'Win7：区域和语言 🞂 键盘和语言 🞂 更改键盘')

#### ** XP **

![系统语言和键盘](_media\lang-and-kbd-xp.webp 'XP：区域和语言选项 🞂 语言 🞂 详细信息')

在 XP 系统上，还需要勾选“将高级文字服务支持应用于所有程序”，SP2 以下还需安装 wic 组件，才能以 TSF 模式运行输入法。

<!-- tabs:end -->

### 启动

第一步（如果想要以外挂模式启动，请跳过此步）：把光标定位到任意文本框，然后如图在任务栏托盘或语言工具栏中切换到 Yong 输入法键盘（也可以用快捷键切换，一般是<kbd>Ctrl</kbd><kbd>Shift</kbd>或<kbd>Win</kbd><kbd>Space</kbd>）。如果系统只有 Yong 输入法一个键盘，则不需要切换键盘，此步跳过。

<!-- tabs:start -->

#### ** Win11 **

![切换系统键盘](_media\run-tsf-on-win11.webp 'Win10')

#### ** Win10 **

![切换系统键盘](_media\run-tsf-on-win10.webp 'Win10')

#### ** Win7 **

![切换系统键盘](_media\run-tsf-on-win7.webp 'Win7')

#### ** XP **

![切换系统键盘](_media\run-tsf-on-xp.webp 'XP')

<!-- tabs:end -->

第二步：启动输入法主程序（可以从开始菜单启动，或者运行程序目录下的 w64/yong.exe）。

第三步：呼出小小输入法的状态条。

<!-- tabs:start -->

#### ** Win8 或更新的系统 **

把光标定位到任意文本框，即可使用<kbd>Ctrl</kbd><kbd>Space</kbd>快捷键，呼出（或隐藏）小小输入法的状态条。

如果成功安装了 TSF 模块，也可以鼠标点击任务栏托盘的「英」来呼出（或隐藏）小小输入法状态条。

#### ** Win7 和 XP **

使用<kbd>Ctrl</kbd><kbd>Space</kbd>快捷键，呼出（或隐藏）小小输入法的状态条。

如果成功安装了 TSF 模块，可以鼠标点亮任务栏托盘的小小输入法图标，来呼出（或隐藏）小小输入法的状态条。

<!-- tabs:end -->

> [!TIP|label:判断输入法当前运行模式的方法]
> 右击输入法状态条，如果看到“TSF 模式未生效”的菜单项，说明正以外挂模式运行，否则以 TSF 模式运行。

### 退出 · 重启 · 重载

这些命令都包含在输入法状态条的右键菜单中。

> [!THXNOTE|label:重载 vs 重启]
> **重载**是指在不**重启**输入法的情况下，重新载入码表文件和大部分配置项。鼠标中键单击输入法状态条也可以触发重载。

### 升级

安装到计算机里的小小星空主要由两部分组成：小小输入法主程序 + 星空方案码表。

前者可以通过**右击输入法状态条 🞂 小小输入法主程序（ooxx） 🞂 更新主程序**来自动从小小输入法的服务器获取更新。

后者目前没有自动升级方式，只能在本项目发布新版本后，手动下载安装程序或者项目文件来进行升级。

> [!THXNOTE|label:为什么码表不能自动升级？]
> 1. 目前星空系列方案的官方码表已经稳定，基本不需要升级。
> 2. 官方码表仅供参考，我们更鼓励用户定制并维护自己的码表。此外，用户可以考虑使用[小小输入法为提供的免费同步空间](https://yong.dgod.net/read.php?tid=651)来同步个人码表和设置。
> 3. 国内网络环境不稳定，如果不购买服务器，难以建立稳定且免费的升级通道。我曾经为小小星空（当时叫小小键道）写过一个自动升级程序「千年轮」，但是因为这个原因，后面还是中止维护了。未来如果这一方面有所改善，可能会恢复。

### 卸载

从开始菜单、控制面板或者程序目录执行卸载程序即可。

> [!ATTENTION|label:在开始菜单里找不到卸载程序的快捷方式？]
> 由于 Win10 的一个[疑似 bug](https://answers.microsoft.com/zh-hans/windows/forum/all/%E7%A8%8B%E5%BA%8F%E7%9A%84%E5%8D%B8%E8%BD%BD/0b57356b-e988-486e-b863-1cf63e0cf0d2)，在开始菜单中可能无法显示卸载程序，你可以改为运行程序目录下的卸载程序。

## ** Android **

### 安装

方式一：使用[小小星空输入法 Android 版安装程序][小小星空网盘]。

方式二：先安装[原版小小输入法 Android 版][小小输入法网盘]，然后下载[:fa fa-github: 本项目源代码][小小星空仓库]，将 home 目录里的内容（最关键的是 mb 目录）复制到 sdcard/yong/.yong 目录中，再将 yong-android.ini 更名为 yong.ini（替换掉原来的 yong.ini）。

> [!ATTENTION|label:找不到目录？]
> sdcard/yong/.yong 是一个隐藏目录，系统自带的文件管理器有可能看不到它。

### 启动

1. 打开桌面上的 Yong 输入法图形设置界面，并授予有关权限，包括：悬浮窗权限（必须的）、所有文件管理权限（必须的）、访问媒体文件、接收短信、麦克风权限、读取联系人、摄像头、读取剪贴板等。
2. 在 Yong 输入法图形设置界面中进行个性化设置（例如在“输入法”页选择默认输入方案，在“安卓”页开启有关功能；注意每个页面修改后要点右上角的保存才会生效）。

![图形设置界面](_media\settings-android.webp 'Yong 输入法 Android 版的图形设置界面')

3. 在手机系统设置的输入法管理页面（可通过 **Yong 输入法图形配置界面 🞂 安卓 🞂 设置系统输入法**快速打开），启用 Yong 输入法键盘。
4. 在任意文本框呼出输入法键盘，并切换至 Yong 输入法键盘（如果无法切换，就在手机系统设置的输入法管理页面中修改当前输入法）。如果顺利的话，你将看到 Yong 输入法的键盘，并且手机里会生成 sdcard/yong/.yong 目录。

### 退出

长按手机桌面上 Yong 输入法图标，在“应用详情”中强行停止即可。

### 升级

如果你是用方式一安装的，那么只能手动下载小小星空的 apk 来升级。

如果你是用方式二安装的，那么可以在 **Yong 输入法图形设置界面 🞂 服务 🞂 更新**中下载最新的原版小小输入法安装包来升级。

不管采用何种方式，sdcard/yong/.yong 目录都不会被覆盖，因此在升级之前你可以根据实际需要删除或保留该目录。

### 卸载

像卸载普通 app 一样卸载后，还需要删除 sdcard/yong 目录。

## ** Linux **

### 安装

<br>

> [!THXNOTE|label:并非通解]
> Linux 有很多发行版、桌面环境和输入法框架，本文只介绍 Debian 12 + GNOME Shell + IBus 环境下的安装方法，其他环境请参考[小小输入法官方文档](https://yong.dgod.net/read.php?tid=6)。

1. 下载并解压[原版小小输入法 Linux 版][小小输入法网盘]（如 yong-lin-3.0.0.1.7z），解压后把里面的 yong 程序目录放到你喜欢的目录（如 /usr/local 或者 home 目录）。
2. 确保已安装了 im-config 包，然后进入 yong 程序目录，执行安装指令 sudo ./yong-tool.sh --install。
3. 注销并重新登录桌面，在**系统设置 🞂 键盘**里添加输入源，把中文 (Yong) 添加进去。

![添加输入源](_media\kbd-linux.webp '添加输入源')

4. 依次执行一次“[启动](#启动)”和“[升级](#升级)”的步骤。

### 启动

打开文本编辑器，右上角切换到中文 (Yong)，按 Ctrl+Space 呼出输入法状态条。

![运行输入法](_media\run-on-linux.webp '运行输入法')

### 退出

右击小小输入法状态条，选择退出即可。

### 升级

[退出](#退出)小小输入法，下载[:fa fa-github: 本项目源代码][小小星空仓库]，将 home 目录里的内容（最关键的是 mb 目录和 entry 目录）复制到配置目录（~/.yong），再把 yong-win.ini 重命名为 yong.ini（替换掉原本的 yong.ini）。

### 卸载

进入程序目录，并执行命令 sudo ./yong-tool.sh --uninstall。

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