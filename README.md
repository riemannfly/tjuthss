# TJUTHSS

_TJUTHSS_ fork 了张井和余蓝涛等同学编写的天津大学学位论文模板 [tjuthesis][tjuthesis]。目前只有为自己准备的 _博士_ 版本。


## 注意

_TJUTHSS_ 并不是一个重新实现的模板，因为 _[tjuthesis][tjuthesis]_ 已经实现了大部分本校的要求。

## 目录和文件说明

1. 主文件 `tjumain.tex`
2. 封面、独创性声明、学位论文版权使用授权书、摘要 `perface/*`
3. 正文 `body/*`
4. 插图 `figures/*`
5. 参考文献 `references/*`
6. 附录 `appendix/*`
7. 论文格式配置文件 `setup/*`, `gb_452.cpx`, `TJUThesis.bst`
8. Makefiles `MakefileInclude\*`, `Makefile`, `*.bat`
9. 天津大学学位论文格式要求 `OfficialDocs\*`
0. 字体 `*.ttf`, `*.ttc`

## 运行

获取该 _repo_ :

    git clone git@github.com:itolssy/tjuthesis.git
 
修改 **preface/cover.tex** 中的相关个人信息和摘要，修改正文（ **body/** ）、参考文献（ **references/** ）、附录（ **appendix/** ）、以及 **tjumain.tex** 中的相关信息，图片放在 **figures** 目录里，然后编译（默认使用 `pdflatex` ）:

    make
    
清除中间内容:
   
    make clean


## Tips

1. `tjumain` 本身提供了一些帮助，可以读一下。
2. 一个据说不错的[中文LaTeX课程](http://math.ecnu.edu.cn/~latex/ "LaTeX 科技排版")，华东师大出品。
3. 包太雷的 [LaTeX Notes](http://www.dralpha.com/zh/tech/lnotes2.pdf "雷太赫排版系统简介 v2.0") ([源码](http://www.dralpha.com/zh/tech/lnotes2.zip)) 是本漂亮的小册子。


## FAQ

1. Windows 与 Linux 某发行版下编译有问题
 * 尚未在 _Win_ 与 _Linux_ 实验过，欢迎补充。目前仅在 _OSX_ 下个人使用，以下提到的问题也是基于 _OSX_。
 * [tjuthesis][tjuthesis] 主要是在 _Win_ 下编写的，可以尝试原版。
2. 中文字体有问题
 * 请确认已安装相关字体，并同步修改了相关文件（如`/usr/local/texlive/2013/texmf-dist/tex/latex/ctex/fontset/`中的文件）。
 * 项目根目录中放置了 _宋体_ 等六个 _Win_ 中的字体文件。


## TODO

* 继续深度修改使更和谐易用
* 添加 _本科_ 和 _硕士_ 版本

[tjuthesis]: https://code.google.com/p/tjuthesis/ "about tjuthesis"
