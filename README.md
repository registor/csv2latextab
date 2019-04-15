# 通过CSV文件生成LaTeX表格的几种方法

[![Travis build](https://travis-ci.org/ustctug/ustcthesis.svg?branch=master)](https://travis-ci.org/ustctug/ustcthesis)
[![Github downloads](https://img.shields.io/github/downloads/ustctug/ustcthesis/total.svg)](https://github.com/ustctug/ustcthesis/releases)
[![GitHub release](https://img.shields.io/github/release/ustctug/ustcthesis/all.svg)](https://github.com/ustctug/ustcthesis/releases/latest)
[![GitHub commits](https://img.shields.io/github/commits-since/ustctug/ustcthesis/latest.svg)](https://github.com/ustctug/ustcthesis/commits/master)

本项目通过实例说明如果通过CSV文件(逗号分割值文件)生成LaTeX表格的几种方法，兼容最新版的TeXLive、MacTeX 、MikTeX发行版，支持跨平台使用。

CSV文件称逗号分隔值(Comma-Separated Values, CSV,有时也称为字符分隔值,因为分隔字符也可以不是逗号)文件，以纯文本形式存储表格数据 (数字和文本)。纯文本意味着该文件是一个字符序列，
不含必须像二进制数字那样被解读的数据。CSV 文件由任意数目的记录组成，记录间以某种换行符分隔；每条记录由字段组成，字段间的分隔符是其它字符或字符串，最常见的是逗号或制表符。通常，所有记录
都有完全相同的字段序列。 CSV文件都是纯文本文件，可以使用记事本、 Excel等软件进行生成或编辑，是一种比较方便的数据管理方式。在LaTeX中可以采用csvsimple、pgfplotstable、datatool、csvtools等宏
包直接使用CSV文件的数据生成LaTeX表格。

注意：

1. 本模板要求 TeXLive、MacTeX、MikTeX 不低于 2018 年的发行版，并且尽可能升级到最新。

3. **不支持** [CTeX 套装](http://www.ctex.org/CTeXDownload)。


## 编译文档

- 编译示例文档 `main.pdf`：
1. 支持minted代码排版宏包
   ```
   latexmk -xelatex -shell-escape main.tex
   ```
2. 不支持minted代码排版宏包
   ```
   latexmk -xelatex main.tex
   ```
3. 在与`main.tex` 同级目录下存在`.latexmkrc` 脚本文件的情况下，执行：
   ```
   latexmk
   ```
- 如需清理论文编译过程中的临时文件，可以：
   ```
   latexmk -c
   ```

## 反馈问题

如果发现代码有问题，请按照以下步骤操作：

1. 将 TeX 发行版和宏包升级到最新，并且将模板升级到 Github 上最新版本，
查看问题是否已经修复；
2. 在 [GitHub Issues](https://github.com/registor/csv2latextab/issues)
中搜索该问题的关键词；
3. 在 [GitHub Issues](https://github.com/registor/csv2latextab/issues)
中提出新 issue，并回答以下问题：
    - 使用了什么版本的 TeX Live / MacTeX / MikTeX ？
    - 具体的问题是什么？
    - 正确的结果应该是什么样的？
    - 是否应该附上相关源码或者截图？
4. 联系作者：西北农林科技大学信息工程学院耿楠


## 更多资料

- [csvsimple宏包说明](https://ctan.org/pkg/csvsimple)
- [csvsimple GitHub](https://github.com/T-F-S/csvsimple)
- [pgfplotstable宏包说明](https://ctan.org/pkg/pgfplotstable)
- [datatool宏包说明](https://ctan.org/pkg/datatool)

