# 武汉大学遥感院硕士研究生毕业论文 LaTeX 模板

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Last Commit](https://img.shields.io/github/last-commit/whutug/whu-thesis.svg)](https://github.com/whutug/whu-thesis/commits/)
[![Overleaf](https://img.shields.io/badge/overleaf-whuthesis-green.svg)](https://www.overleaf.com/latex/templates/wuhan-university-latex-undergraduate-thesis-template/kpystysgbgmr)
[![](https://github.com/whutug/whu-thesis/workflows/LaTeX%20Compile/badge.svg)](https://github.com/whutug/whu-thesis/actions)

本项目为武汉大学遥感信息工程学院硕士研究生毕业论文 LaTeX 模板。

本科生、博士请勿直接使用，但可根据本模板更改cls文件中对应的代码。

**声明** 该模板为我在撰写毕业论文时根据学院张薇老师提供的word模板对[WHU-TUG](https://github.com/whutug)提供[原始模板](https://github.com/whutug/whu-thesis)进行更改得到。由于本人LaTeX技术有限，我在修改时仅对原始模板中我所发现的与学院word文档不同之处，且我有修改能力的地方进行了改动，因此，该模板不可避免与学院标准word文档间存在一定差异。如果介意，请直接使用学院的word模板，或者在此模板基础上进一步修改。谢谢大家~
## 样例展示

<p align="center">
  <img src="https://github.com/yaochenzhu/whu-rsie-master-thesis/blob/main/figures/demo.png" width="800px">
</p>

本项目LaTeX模板编译得到的正文样例可以参照 [whu-thesis-demo](whu-thesis-demo.pdf)

张薇老师提供的word模板可以参照[遥感信息工程学院学术学位硕士论文撰写格式](学术学位硕士论文撰写格式.doc)


## 如何使用

推荐两种方式进行编辑和编译：

* [本地编译](#本地编译)
* [Overleaf 在线编译](#overleaf-在线编译)

### 本地编译

本地编译需要安装 TeX 发行版软件, 具体可参见 [本地安装使用指南](https://github.com/mtobeiyf/whu-thesis/wiki/%E6%9C%AC%E5%9C%B0%E5%AE%89%E8%A3%85%E4%B8%8E%E7%BC%96%E8%AF%91)

### Overleaf 在线编译

[![Overleaf](https://img.shields.io/badge/overleaf-whuthesis-green.svg)](https://www.overleaf.com/latex/templates/wuhan-university-latex-undergraduate-thesis-template/kpystysgbgmr)

[Overleaf](https://www.overleaf.com/) 是一个简洁的在线 LaTeX 编辑器。无需安装，实时共享，版本控制。该模板支持了 Overleaf 的在线编辑，可以从上面的模板链接直接创建自己的项目。

使用该模板时，需要设置 `XeLaTeX`为编译器，具体步骤请查看 [Overleaf 在线编辑](https://github.com/mtobeiyf/whu-thesis/wiki/Overleaf-%E5%9C%A8%E7%BA%BF%E7%BC%96%E8%BE%91)

<p align="center">
  <img src="https://github.com/yaochenzhu/whu-rsie-master-thesis/blob/main/figures/demo_overleaf.png" width="800px">
</p>

## 注意事项

*  **参考文献**： 在使用前，请将whu-thesis-demo.tex文件中用于显示全部参考文献的\nocite{*}语句删除。

* **论文使用授权书**： 对于论文使用授权书，请直接填写并替换page文件夹下的authorization.pdf。

* **字体不一致的问题**： 本LaTeX模板在使用overleaf进行编译时，所有的中文字体均使用fandol字体。这与windows自带的中文字体存在不同。因此，在正式提交论文电子版前，请将模板下载到windows主机进行本地编译。如果编译后中文字体仍为fandol字体，请手动将cls文件中688行cjk-font  .initial:n = fandol语句改为cjk-font  .initial:n = windows，再按照xelatex -> bibtex -> xelatex -> xelatex的顺序进行编译即可。

* **纸质版空白页生成的问题**： 在论文定稿准备提交纸质版打印前，请将whu-thesis-demo.tex文件中\renewcommand{\cleardoublepage}{\clearpage}语句注释，以按格式要求正确生成空白页；

* **未来展望**： 如果以后学院出了新的模板，authorization，innovation等不出现在论文目录中的页面发生了变化，你永远可以从模板摘出对应页，填好之后保存成pdf，再在模板对应位置通过\includepdf[]命令将其加入论文（手动狗头）。

</details>

## 主要改动日志 

* **封面**：按学院word模板将中文封面上方横线改为密集虚线，并重构英文封面；

* **摘要** : 按学院word模板修改了中英文关键词的字体；

* **论文使用授权书** ： 从学院word模板中摘出对应页，保存成pdf之后插入论文；

* **目录** ： 按学院word模板修改了目录页的字体与格式；

* **攻硕期间参与的课题情况** ： 按学院word模板添加了参与课题情况；

* **全局**：按学院word模板更改了论文页边距，页眉页码的边距与字体，各章节标题格式字体与段前后间距，公式前后行距，图表公式标号等。

## 致谢

* 感谢[WHU-TUG](https://github.com/whutug)小组的无私奉献，为我们提供论文的原始模板；


* 感谢IIP Lab ZYH同学。 作为本项目唯一的“乙方”，为本模板的撰写提供了很多宝贵的意见。
