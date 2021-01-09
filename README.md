# my-cv

[![Build Status](https://travis-ci.com/eshwen/my-cv.svg?branch=master)](https://travis-ci.com/eshwen/my-cv) [![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/eshwen/my-cv)](https://github.com/eshwen/my-cv/releases/latest) ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/eshwen/my-cv)

Quick download of pdf(s): [![GitHub Releases (by Asset - pdf)](https://img.shields.io/github/downloads/eshwen/my-cv/latest/Eshwen_Bhal_CV.pdf?color=ff69b4)](https://github.com/eshwen/my-cv/releases/latest/download/Eshwen_Bhal_CV.pdf) [![GitHub Releases (by Asset - pdf academic)](https://img.shields.io/github/downloads/eshwen/my-cv/latest/Eshwen_Bhal_CV_academic.pdf?color=ff69b4)](https://github.com/eshwen/my-cv/releases/latest/download/Eshwen_Bhal_CV_academic.pdf) [![GitHub Releases (by Asset - pdf data science)](https://img.shields.io/github/downloads/eshwen/my-cv/latest/Eshwen_Bhal_CV_data_science.pdf?color=ff69b4)](https://github.com/eshwen/my-cv/releases/latest/download/Eshwen_Bhal_CV_data_science.pdf) [![GitHub Releases (by Asset - pdf research)](https://img.shields.io/github/downloads/eshwen/my-cv/latest/Eshwen_Bhal_CV_research.pdf?color=ff69b4)](https://github.com/eshwen/my-cv/releases/latest/download/Eshwen_Bhal_CV_research.pdf) [![GitHub Releases (by Asset - pdf software)](https://img.shields.io/github/downloads/eshwen/my-cv/latest/Eshwen_Bhal_CV_software.pdf?color=ff69b4)](https://github.com/eshwen/my-cv/releases/latest/download/Eshwen_Bhal_CV_software.pdf)

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

There is also a template for a cover letter styled in the same way as the CV: [cover_letter.tex](cover_letter.tex). A pdf can be generated in the same manner as the CV.

The subdirectory [cv_targeted_industries/](cv_targeted_industries/) contains tex files that build more targeted versions of the CV, swapping out the more generic sections in [sections/](sections/) for ones that highlight particular skills or experience related to those fields. They utilise the `subfiles` package to allow the preamble from [cv.tex](cv.tex), meaning compilation and style, etc. will be consistent across each version. The magic argument `%!TeX root = <file>` means `<file>` will be the one compiled in an editor like Visual Studio Code. Otherwise, compilation on the command line uses the same syntax as above.
