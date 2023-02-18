# my-cv

[![Build Status](https://travis-ci.com/eshwen/my-cv.svg?branch=master)](https://travis-ci.com/eshwen/my-cv) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/eshwen/my-cv)](https://github.com/eshwen/my-cv/releases/latest) ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/eshwen/my-cv)

[![GitHub Releases (by Asset - pdf)](https://img.shields.io/github/downloads/eshwen/my-cv/latest/Eshwen_Bhal_CV.pdf?color=ff69b4)](https://github.com/eshwen/my-cv/releases/latest/download/Eshwen_Bhal_CV.pdf)

My CV in LaTeX.

This template has been downloaded from: <https://github.com/posquit0/Awesome-CV> with some changes from unmerged pull requests

Original author: Claud D. Park [posquit0.bj@gmail.com](mailto:posquit0.bj@gmail.com), <http://www.posquit0.com>

Modifications to template by: Junhao Dong [junhao.dong96@gmail.com](mailto:junhao.dong96@gmail.com), Eshwen Bhal [milanman.eshb@gmail.com](mailto:milanman.eshb@gmail.com)

Template license: CC BY-SA 4.0 (<https://creativecommons.org/licenses/by-sa/4.0/>)

## Instructions

Clone this repository. If running with, e.g., TeX Live on macOS, you will need to install the `Roboto` fonts. Just double-click on the `.ttf` files in [fonts/](fonts/) and they will install. The fonts may be installed by default if using an online editor like Overleaf (though I haven't tested whether this is true).

Compilation must be done with `XeLaTeX` or `LuaLaTeX` because of the requirements of the `fontspec` package (i.e., you cannot use `pdflatex`).

With the TeXShop IDE, you can just hit either the **LaTeX** or **XeLaTeX** options in the drop down menu next to **Typeset**, then hit the **Typeset** button.

The same functionality is possible using Visual Studio Code with the **LaTeX Workshop** extension. The magic argument `%!TEX TS-program = xelatex` in [cv.tex](cv.tex) should allow you to just press **Build LaTeX Project**.

In PyCharm, a run configuration in [cv.run.xml](./.run/cv.run.xml) allows the same one-click run. To view the output PDF, a PDF viewer plugin may need to be installed.

In the terminal, assuming the relevant implementation is installed with your TeX distribution, you can just run

```sh
xelatex cv.tex
```

or

```sh
lualatex cv.tex
```

There is also a template for a cover letter styled in the same way as the CV: [cover_letter.tex](cover_letter.tex). A pdf can be generated in the same manner as the CV.
