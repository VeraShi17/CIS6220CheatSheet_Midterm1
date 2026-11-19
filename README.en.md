# CIS6220 Cheat Sheet — Midterm 1

[简体中文](README.md) | **English**

A CIS 6220 Midterm 1 study cheat sheet with bilingual Chinese–English notes and formulas, typeset in a compact five-column A4 landscape layout using LaTeX.

## Template credit

The layout is adapted from [COMP5310_cheatsheet.tex](https://github.com/Purestone/chitshit/blob/main/COMP5310_cheatsheet.tex) in [Purestone/chitshit](https://github.com/Purestone/chitshit). Thanks to the original author for sharing the template.

Credit for the original layout belongs to its author. This repository adjusts the page layout and Chinese-language support, and replaces the body with CIS 6220 study notes.

## Layout changes

The original A4 landscape format, five columns, gray topic headers, and blue subtopic headings are retained. The main changes are:

| Setting | Upstream template | This project |
| --- | --- | --- |
| Top and bottom margins | 1 cm each | 0.5 cm each; left and right margins remain 0.75 cm each |
| Body font size / line spacing | 5 pt / 6 pt | 4 pt / 5 pt for greater content density |
| Chinese support | No dedicated Chinese font configuration | Adds `xeCJK` with Chinese sans-serif font fallbacks: Noto Sans CJK SC → FandolHei-Regular → SimHei |
| Space before topic headers | `\medskip` | `\smallskip` for tighter heading spacing |

## Compilation

The main source file is [`main.tex`](main.tex). Compile with **XeLaTeX** to support the mixed Chinese–English text:

```sh
xelatex -interaction=nonstopmode main.tex
```

In Overleaf, set the compiler to **XeLaTeX** and the main document to `main.tex`. The build environment needs at least one of the Chinese fonts listed in the table above.

## Template license

The upstream template is distributed under the MIT License. Its original copyright notice and full license text are preserved in [`LICENSE.template`](LICENSE.template).
