# Version v0.1
The aim of this UGent Beamer theme:
* A theme that closely resembles the official UGent Powerpoint/Keynote presentation themes.
* Similar theme options as the depreciated UGent Beamer theme.
* Ease-of-use for the average Beamer user.

Requires the packages [sfmath](https://ctan.org/pkg/sfmath),
[helvet](https://ctan.org/pkg/helvet) and [PGF/TikZ](https://ctan.org/pkg/pgf)
to be installed in your LaTeX distribution.

Demo
----
A full example is available. Refer to `example/example.tex` and `example/example.pdf`. Or click [here](https://github.com/driesbenoit/ugent-beamer/blob/master/example/example.pdf).

![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-example-02.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-example-03.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-example-04.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-example-05.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-example-11.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-example-17.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-example-20.png)

Download
========
Download the latest release by following [this](https://github.com/driesbenoit/ugent-beamer/releases) link.

Installation
============
The theme is an addendum for the LaTeX beamer class, hence it is assumed that you have a running LaTeX installation together with the beamer package and its dependencies.

Once you have the files, all that is required for the theme to work is putting the files into a directory where LaTeX can find them. This boils down to mimicking the so called TDS (or TeX Directory Structure).

Ad-hoc installation 
-------------------
After downloading, copy the files named beamer*ugent.sty, together with all *.png files from the image folder, into the same folder as your LaTeX source file.

Then include the theme by writing:
```latex
\documentclass{beamer}

\usetheme{ugent}
```
in the preamble of your document.

Installation
------------
In case you're using your favorite flavor of Unix (and/or TeX Live) you need to have a local directory (this will probably be ~/texmf/) and you need to place all the files from the theme folder in the directory ~/texmf/tex/latex/beamer/themes/ugent/, finishing it by running texhash.

If on the other hand you're on Windows (probably MiK\TeX) the walkthrough at [this url](http://docs.miktex.org/manual/localadditions.html) explains thoroughly and with many pictures how to create a local installation. Don't forget to Refresh FNDB as explained [here](http://docs.miktex.org/manual/configuring.html#fndbupdate).

License
=======
This software is released under the [GNU GPL v3.0 License](https://www.gnu.org/licenses/gpl-3.0.en.html).

Contacts
========
If you are enjoying this theme please share it with your friends or colleagues!

Any suggestions, comments, criticism or appreciation are welcome!
