# CIS6220 Cheat Sheet — Midterm 1

**简体中文** | [English](README.en.md)

CIS 6220 期中一复习速查表，采用 A4 横向五栏的紧凑 LaTeX 排版，整理中英文学习笔记与公式。

## 模板来源

本项目的排版基于 [Purestone/chitshit](https://github.com/Purestone/chitshit) 中的 [COMP5310_cheatsheet.tex](https://github.com/Purestone/chitshit/blob/main/COMP5310_cheatsheet.tex) 调整而来。感谢原作者提供模板。

原始排版设计归原作者所有。本仓库在其基础上调整了版面与中文支持，并将正文替换为 CIS 6220 的复习内容。

## 排版调整

沿用原模板的 A4 横向五栏结构、灰底主题标题及蓝色小标题，主要调整如下：

| 项目 | 上游模板 | 本项目 |
| --- | --- | --- |
| 上下页边距 | 各 1 cm | 各 0.5 cm；左右仍为各 0.75 cm |
| 正文字号 / 行距 | 5 pt / 6 pt | 4 pt / 5 pt，提高内容密度 |
| 中文支持 | 无专门的中文字体配置 | 加入 `xeCJK`，配置中文无衬线字体及回退顺序：Noto Sans CJK SC → FandolHei-Regular → SimHei |
| 主题标题前间距 | `\medskip` | `\smallskip`，压缩标题间距 |

## 编译

主文件为 [`main.tex`](main.tex)。请使用 **XeLaTeX** 编译，以支持中英混排：

```sh
xelatex -interaction=nonstopmode main.tex
```

在 Overleaf 中，将项目的编译器设为 **XeLaTeX**，主文件设为 `main.tex`。编译环境需安装上表列出的至少一种中文字体。

## 模板许可

上游模板采用 MIT 许可证。原作者的版权声明与完整许可文本保留在 [`LICENSE.template`](LICENSE.template) 中。
