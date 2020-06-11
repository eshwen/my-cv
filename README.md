# my-cv

[![Build Status](https://travis-ci.com/eshwen/my-cv.svg?branch=master)](https://travis-ci.com/eshwen/my-cv) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/eshwen/my-cv)](https://github.com/eshwen/my-cv/releases/latest) ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/eshwen/my-cv)

Quick download of pdf: [![GitHub Releases (by Asset - pdf)](https://img.shields.io/github/downloads/eshwen/lab-book/latest/Eshwen_Bhal_CV.pdf?color=ff69b4)](https://github.com/eshwen/my-cv/releases/latest/download/Eshwen_Bhal_CV.pdf)

My CV in LaTeX.

This template has been downloaded from: <https://github.com/posquit0/Awesome-CV> with some changes from unmerged pull requests

Original author: Claud D. Park [posquit0.bj@gmail.com](mailto:posquit0.bj@gmail.com), <http://www.posquit0.com>

Modifications to template by: Junhao Dong [junhao.dong96@gmail.com](mailto:junhao.dong96@gmail.com), Eshwen Bhal [eshwen.bhal@bristol.ac.uk](mailto:eshwen.bhal@bristol.ac.uk)

Template license: CC BY-SA 4.0 (<https://creativecommons.org/licenses/by-sa/4.0/>)

## Instructions

Clone this repository. If running with, e.g., TeX Live on macOS, you will need to install the `Roboto` fonts. Just double-click on the `.ttf` files in [fonts/](fonts/) and they will install. The fonts may be installed by default if using an online editor like Overleaf (though I haven't tested whether this is true).

Compilation must be done with `XeLaTeX` or `LuaLaTeX` because of the requirements of the `fontspec` package (i.e., you cannot use `pdflatex`). With the TeXShop IDE, you can just hit either the **LaTeX** or **XeLaTeX** options in the drop down menu next to **Typeset**, then hit the **Typeset** button. The same functionality is possible using Visual Studio Code with the **LaTeX Workshop** extension. The magic argument `%!TEX TS-program = xelatex` in [cv.tex](cv.tex) should allow you to just press **Build LaTeX Project**.

In the terminal, assuming the relevant implementation is installed with your TeX distribution, you can just run

```sh
xelatex cv.tex
```

or

```sh
lualatex cv.tex
```

## To do

- Send around to other people (parents, other colleagues, Henning and Joel?)
- Add a pdf copy to profile on LinkedIn once ready?
- Send final copy to people at Imagination Technologies
- Add 3-4 paragraphs about PhD (intro to topic and what I'm doing, highlighting skills and experience I've gained) on a new page(s) and send that copy to Peter Skelton at Ab Initio
