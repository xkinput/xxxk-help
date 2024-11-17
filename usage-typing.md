# 基本功能

当你了解了一种星空系列方案（可参阅[方案介绍](schema.md)）后，便可以开始利用小小星空输入法进行打字。

## 启用方案

在图形化配置程序 `yong-config.exe`（可通过点击输入法状态条上的齿轮图标，或者输入法状态条的右键菜单，或者键入命令直通车 `ooxx` 来启动）中，加载你想使用的方案（如下图左），卸载不想使用的方案（如下图右）。

![管理方案](_media\config-manage-schema.png)

?> 可以放心地卸载内置的方案，卸载后是可以重新加载回来的。

接着，切换到你想使用的方案。

* 切**换**方案：<kbd>Ctrl</kbd><kbd>Shift</kbd><kbd>H</kbd>，或点击输入法状态条上的方案名（有的皮肤不显示方案名）

## 方案学习

* 看**入门**教程：`oorm`，或通过输入法状态条右键菜单
* 上**官网**：`oogw`，或通过输入法状态条右键菜单
* **键盘**图：三种方法查看当前方案的键盘布局：①<kbd>Ctrl</kbd><kbd>Shift</kbd><kbd>M</kbd>；②命令直通车 `oojp`；③通过输入法状态条右键菜单
* 逆查编码：复制想查询编码的字词，然后 <kbd>Ctrl</kbd><kbd>?</kbd>
* 联网查字：把想查询的字词打出到候选，然后 <kbd>Ctrl</kbd><kbd>?</kbd>
* 笔画引导键：`` ` ``（位于数字`1`键左侧），例如 `ddh = 氵`
* 万能键：`~`，例如 `bmov~~ = 辫`
* 临时全拼引导键：`e`（仅用于星空两笔）
* **单**字模式：<kbd>Ctrl</kbd><kbd>Shift</kbd><kbd>D</kbd>切换，开启后不能打词，适合练习单字

?> 遇到不会打、不认识的字词，除了用小小输入法自带的逆查编码、联网查字功能外，还可以使用在线[字词查询](res#字词查询)工具。

## 状态切换

* **简**繁切换：<kbd>Ctrl</kbd><kbd>Shift</kbd><kbd>J</kbd>
* 全半角切换：<kbd>Ctrl</kbd><kbd>Space</kbd>
* 中英文标点模式切换：<kbd>Ctrl</kbd><kbd>.</kbd>（或者按住 <kbd>Alt</kbd> 临时切换为英文标点模式）
* 临时英文模式：按左 <kbd>Ctrl</kbd>，则下次输入会变成临时英文模式。这是一种特殊的输入模式，在该模式下，你可以快速输入大写数字、日期、英文，甚至进行数学运算。注意：在临时英文模式下打英文，不能直接用数字键来上屏指定候选项，而要用 <kbd>Alt</kbd> + 数字键。
![临时英文模式](_media\en-mode.png)

## 特殊字符

* 两分输入：在星空系列方案下，用 `u` 引导，如 `ulyly = 龖`（两分方案规则参阅[方案介绍：字海两分](schema-zhlf)）
* 火星文（菊花文）模式：<kbd>Ctrl</kbd><kbd>Shift</kbd><kbd>Alt</kbd><kbd>H</kbd> 切换
* 软键盘：通过输入法状态条呼出。右击符号键盘，可切换符号类别  
* **符**号大全：`of` 引导各类符号，`ol` 引导 LaTeX，`or` 引导日文假名（平文式罗马音），`op` 引导拼音和注音符号……按 `o` 即可看到提示
* 快捷符号：`;` 引导，可以快速输入少量常用符号
  <details>
      <summary>点我查看快捷符号清单</summary>
      <style type="text/css">
      .tg  {border-collapse:collapse;border-spacing:0;}
      .tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
        overflow:hidden;padding:5px 5px;word-break:normal;}
      .tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
        font-weight:normal;overflow:hidden;padding:5px 5px;word-break:normal;}
      .tg .tg-kkmc{border-color:inherit;font-family:"Arial Black", Gadget, sans-serif !important;text-align:left;vertical-align:top}
      .tg .tg-sej6{border-color:inherit;font-family:"Lucida Console", Monaco, monospace !important;text-align:left;vertical-align:top}
      </style>
      <table class="tg" style="undefined;table-layout: fixed; width: 1209px"><colgroup>
      <col style="width: 121px">
      <col style="width: 121px">
      <col style="width: 121px">
      <col style="width: 121px">
      <col style="width: 121px">
      <col style="width: 121px">
      <col style="width: 121px">
      <col style="width: 121px">
      <col style="width: 120px">
      <col style="width: 121px">
      </colgroup>
      <tbody>
        <tr>
          <td class="tg-kkmc">Q (query)</td>
          <td class="tg-kkmc">W (wave)</td>
          <td class="tg-kkmc">E (enter)</td>
          <td class="tg-kkmc">R (repeat)</td>
          <td class="tg-kkmc">T (退格)</td>
          <td class="tg-kkmc">Y</td>
          <td class="tg-kkmc">U (undo)</td>
          <td class="tg-kkmc">I</td>
          <td class="tg-kkmc">O</td>
          <td class="tg-kkmc">P (破折)</td>
        </tr>
        <tr>
          <td class="tg-sej6">;q  = ？<br>;qo = ¿<br></td>
          <td class="tg-sej6">;w = ～</td>
          <td class="tg-sej6">;e = 回车</td>
          <td class="tg-sej6">;r = 重复</td>
          <td class="tg-sej6">;t = 退格</td>
          <td class="tg-sej6">;y  = ♂<br>;yo = ♀</td>
          <td class="tg-sej6">;u = 撤销</td>
          <td class="tg-sej6">;i = ！</td>
          <td class="tg-sej6">;o  = ·<br>;oo = ……</td>
          <td class="tg-sej6">;p = ——</td>
        </tr>
        <tr>
          <td class="tg-kkmc">A (at)</td>
          <td class="tg-kkmc">S</td>
          <td class="tg-kkmc">D (del)</td>
          <td class="tg-kkmc">F</td>
          <td class="tg-kkmc">G</td>
          <td class="tg-kkmc">H (行)</td>
          <td class="tg-kkmc">J (井 箭)</td>
          <td class="tg-kkmc">K (括号)</td>
          <td class="tg-kkmc">L</td>
          <td class="tg-kkmc">;</td>
        </tr>
        <tr>
          <td class="tg-sej6">;a = @</td>
          <td class="tg-sej6">;s  = &amp;<br>;si = $</td>
          <td class="tg-sej6">;d = Del</td>
          <td class="tg-sej6">;f = “</td>
          <td class="tg-sej6">;g = ”</td>
          <td class="tg-sej6">;h  = END<br>;ho = HOME</td>
          <td class="tg-sej6">;j   = #<br>;ji = ↑<br>;jii = 🞁</td>
          <td class="tg-sej6">;ku = ()<br>;ki = []<br>;ko = {}</td>
          <td class="tg-sej6">;l  = |<br>;lu = /<br>;lo = \<br>;ll = //</td>
          <td class="tg-sej6">;; = ；</td>
        </tr>
        <tr>
          <td class="tg-kkmc">Z</td>
          <td class="tg-kkmc">X</td>
          <td class="tg-kkmc">C (constrain)</td>
          <td class="tg-kkmc">V</td>
          <td class="tg-kkmc">B (百分号)</td>
          <td class="tg-kkmc">N</td>
          <td class="tg-kkmc">M</td>
          <td class="tg-kkmc">,</td>
          <td class="tg-kkmc">.</td>
          <td class="tg-kkmc"></td>
        </tr>
        <tr>
          <td class="tg-sej6">;z = _</td>
          <td class="tg-sej6">;x  = ×<br>;xo = ÷</td>
          <td class="tg-sej6">;c = `</td>
          <td class="tg-sej6">;v  = √<br>;vv = ^</td>
          <td class="tg-sej6">;b   = %<br>;bo  = ‰<br>;boo = ‱</td>
          <td class="tg-sej6">;n = ‘</td>
          <td class="tg-sej6">;m = ’<br></td>
          <td class="tg-sej6">;, = &lt;</td>
          <td class="tg-sej6">;. = &gt;</td>
          <td class="tg-sej6"></td>
        </tr>
      </tbody></table>
  </details>

?> 有些字符需要安装[超大字集](res#超大字集)才能显示。

## 右键菜单

输入法状态条的右键菜单里集成了一些命令，它们也可以通过键入编码来执行：

* `ooxx` 提供与**小小**输入法程序相关的功能：重启小小、配置小小、重载小小、重置小小、退出小小
* `oomb` 快速打开相关**码表**：在线码表、本地码表
* `ooml` 快速打开相关**目录**：程序目录、配置目录
* `oorm` 快速打开在线和本地**入门**说明书
* `oogw` 快速打开**官网**
* `oojp` 快速打开**键盘**图

