# 更新历史

<iframe height='400' scrolling='no' title='小小星空键道词库更新时间线' src='_plugins/echarts-v6.0.0/timeline.html' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'>小小星空键道词库更新时间线</iframe><!-- 250730 -->

## 最近更新

##### [v2.0.9.0-Build20251207](https://github.com/xkinput/xxxk/releases/tag/v2.0.9)

*例行更新。*

* feat: 更新主程序至[2025年12月4日测试版](https://yong.dgod.net/read.php?tid=2)。
* feat: 安卓版“彩”皮肤更新至 251128 版。
* doc: 更新在线文档内容和组件。

##### [v2.0.8.0-Build20251005](https://github.com/xkinput/xxxk/releases/tag/v2.0.8)

*小修小补。*

* feat: 更新主程序至[2025年8月30日测试版](https://yong.dgod.net/read.php?tid=2)。
* feat: 安卓版“彩”皮肤更新至 250522 版。
* doc: 更新在线文档内容和组件。

##### [v2.0.7.0-Build20250512](https://github.com/xkinput/xxxk/releases/tag/v2.0.7)

*小修小补。*

* feat: 更新主程序至[2025年5月12日测试版](https://yong.dgod.net/read.php?tid=2)。
* fix: 因两个功能的快捷键不再兼容，现恢复联网查字和反查编码功能的快捷键为默认。

##### [v2.0.6.0-Build20250508](https://github.com/xkinput/xxxk/releases/tag/v2.0.6)

*修缮文档。*

* feat: 更新主程序至[2025年5月8日测试版](https://yong.dgod.net/read.php?tid=2)。
* doc: 更新在线文档内容和组件（补充关于 Linux 和 Android 的安装使用说明），更新 yong.chm 到 [241222 版](https://yong.dgod.net/read.php?tid=33)。

##### [v2.0.5.0-Build20250426](https://github.com/xkinput/xxxk/releases/tag/v2.0.5)

*日常更新主程序。*

* feat: 更新主程序至[2025年4月12日测试版](https://yong.dgod.net/read.php?tid=2)，在[个别软件里中英文状态切换异常的问题](https://yong.dgod.net/read.php?tid=4932)已被修复。

##### [v2.0.4.0-Build20250111](https://github.com/xkinput/xxxk/releases/tag/v2.0.4)

*继续改进编译流程，方便后续维护。*

* feat: 增加一个新版皮肤（Default5.zip）。
* feat: 更新主程序至[2025年1月10日测试版](https://yong.dgod.net/read.php?tid=2)。
* chore: 编译 xxxk.nsi 时，自动将 xxxkConst.nsh 里的安装包版本号更新到 version.txt 和 menu.ini 里的版本信息。

##### [v2.0.3.0-Build20241216](https://github.com/xkinput/xxxk/releases/tag/v2.0.3)

*主要是增强了可维护性：将输入法主程序与星空方案数据文件分离。*

* refactor: 调整项目目录结构，分成 build（构建工具），data（程序）和 home（数据）。
* chore: 增加 Android 版编译脚本 xxxk.bat，可快速打包生成 apk（参见[开发指南](develop.md)）。
* chore: 优化 Windows 版编译脚本 xxxk.nsi，现在安装包会将数据文件安装到配置目录（而不是程序目录）。
* feat: 现在 Windows 版可以单独更新输入法主程序了（右键菜单 🞂 小小输入法主程序 🞂 更新主程序）。
* feat: 更新小小输入法主程序至2024年12月16日测试版，启用新版小小输入法的启发式造词特性（code_hint），并支持新版小小输入法的云剪贴板功能（`;cc`）。
* docs: 更新 yong.chm。

##### [v2.0.1.0-Build20241124](https://github.com/xkinput/xxxk/releases/tag/v2.0.1)

*主要是跟进小小输入法测试版的更新。暂时只有 Windows 版，Android 版后续再跟进。*

* 更新小小输入法主程序至2024年11月23日测试版。
* 修复安装包无法恢复用户设定的问题。
* 调整安装包文件名，采用纯英文（文件名里的中文字符在上传 github release 时会被吞掉）。
* 移除一些历史遗留文件，减小安装包体积。

##### [v2.0.0.0-Build20241117](https://github.com/xkinput/xxxk/releases/tag/v2.0.0)

*主要是优化了安装包，并跟进这两年小小输入法测试版的更新。暂时只有 Windows 版，Android 版后续再跟进。*

* 调整仓库目录结构，方便后续维护。
* 升级小小输入法程序到 20241116 测试版。
* 重写安装脚本（`app-win/nsis/xxxk.nsi`），简化流程，加强用户权限识别，优先使用 64 位版本输入法等。
* 键道码表跟进 RIME 版，主词条数：121386。
* 更新帮助文档等资料。
* 打包程序由 NSIS2 升级为 NSIS3（详见 [NSIS 更新记录](https://nsis.sourceforge.io/Docs/AppendixF.html)）。