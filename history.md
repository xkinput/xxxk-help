# 更新历史

<iframe height='400' scrolling='no' title='小小星空更新时间线' src='_plugins/echarts-241117/timeline.html' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'>小小星空更新时间线</iframe><!-- v5.3.3 -->

## 最近更新

##### [v2.0.3.0-Build20241216](https://github.com/xkinput/xxxk/releases/tag/v2.0.3)

*主要是增强了可维护性：将输入法主程序与星空方案数据文件分离。*

* refactor: 调整项目目录结构，分成 build（构建工具），data（程序）和 home（数据）。
* chore: 增加 Android 版编译脚本 xxxk.bat，可快速打包生成 apk（参见[开发指南](develop.md)）。
* chore: 优化 Windows 版编译脚本 xxxk.nsi，现在安装包会将数据文件安装到配置目录（而不是程序目录）。
* feat: 现在 Windows 版可以单独更新输入法主程序了（右键菜单 🞂 小小输入法主程序 🞂 更新主程序）。
* feat：更新小小输入法主程序至[2024年12月16日测试版](https://yong.dgod.net/read.php?tid=2)，启用新版小小输入法的启发式造词特性（code_hint），并支持新版小小输入法的云剪贴板功能（`;cc`）。
* docs: 更新 yong.chm。

##### [v2.0.1.0-Build20241124](https://github.com/xkinput/xxxk/releases/tag/v2.0.1)

*主要是跟进小小输入法测试版的更新。暂时只有 Windows 版，Android 版后续再跟进。*

* 更新小小输入法主程序至[2024年11月23日测试版](https://yong.dgod.net/read.php?tid=2)。
* 修复安装包无法恢复用户设定的问题。
* 调整安装包文件名，采用纯英文（文件名里的中文字符在上传 github release 时会被吞掉）。
* 移除一些历史遗留文件，减小安装包体积。

##### [v2.0.0.0-Build20241117](https://github.com/xkinput/xxxk/releases/tag/v2.0.0)

*主要是优化了安装包，并跟进这两年小小输入法测试版的更新。暂时只有 Windows 版，Android 版后续再跟进。*

* 调整仓库目录结构，方便后续维护。
* 升级小小输入法程序到 20241116 测试版。⚠ 此版本输入法在某些应用中以 TSF 模式运行时，会出现**中英文状态切换异常问题：**用中英文切换快捷键（如 SHIFT）切换为英文状态后，再按下任意键，会导致输入法立刻变回中文状态。**临时处理方案：**在这些应用中，使用打开/关闭输入法快捷键（如 CTRL+SPACE）或临时英文模式（如 CTRL）来代替中英文切换快捷键。
* 打包程序由 NSIS2 升级为 NSIS3（详见 [NSIS 更新记录](https://nsis.sourceforge.io/Docs/AppendixF.html)）。
* 重写安装脚本（`app-win/nsis/xxxk.nsi`），简化流程，加强用户权限识别，优先使用 64 位版本输入法等。
* 键道码表跟进 RIME 版，主词条数：121386。
* 更新帮助文档等资料。

##### [v1.0.5.0-Build20220708](https://github.com/xkinput/xxxk/releases/tag/v1.0.5)

* 改进：跟进小小输入法程序组件升级（Windows 版修复了一些程序 bug，Android 版不再支持 32 位）
* 改进：其他微调