# 更新历史

<iframe height='400' scrolling='no' title='小小星空更新时间线' src='_plugins/echarts-241117/timeline.html' frameborder='no' allowtransparency='true' allowfullscreen='true' style='width: 100%;'>小小星空更新时间线</iframe><!-- v5.3.3 -->

## 最近更新

##### [v2.0.0.0-Build20241117](https://github.com/xkinput/xxxk/releases/tag/v2.0.0)

*经测试，该版本的小小输入法在某些应用中以 TSF 模式运行时，会出现中英文状态切换异常的问题：使用中英文切换快捷键（如 SHIFT）切换为英文状态后，再按下任意键，会导致输入法立刻变回中文状态。临时解决方案：使用打开/关闭输入法快捷键（如 CTRL+SPACE）来代替中英文切换快捷键。*

* 调整项目架构为 app-win, data-base 和 data-schema 三个文件夹，方便后续维护
* 升级小小输入法程序到 20241116 版（详见[小小输入法更新记录](http://yong.dgod.net/read.php?tid=2&fid=2)）
* 打包程序由 NSIS2 升级为 NSIS3（详见 [NSIS 更新记录](https://nsis.sourceforge.io/Docs/AppendixF.html)）
* 重写安装脚本（`app-win/nsis/xxxk.nsi`），简化流程，加强用户权限识别等
* 键道码表跟进 RIME 版，主词条数：121386
* 更新帮助文档等资料

##### [v1.0.5.0(pre)-Build20220708](https://github.com/xkinput/xxxk/releases/tag/v1.0.5)

*这是一个预发行版本，只更新了依赖组件，未更新主码表。如果上一版本使用没什么问题，可以不更新到此版。*

* 改进：跟进小小输入法程序组件升级（Windows 版修复了一些程序 bug，Android 版不再支持 32 位）
* 改进：其他微调