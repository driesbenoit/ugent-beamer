# Version v0.1-2
The aim of this UGent Beamer theme:
* A theme that closely resembles the official UGent Powerpoint/Keynote presentation themes.
* Similar theme options as the [depreciated UGent Beamer theme](https://github.com/pbelmans/ugent-beamer) by Pieter Belmans.
* A corporate version, as well as faculty specific versions.
* Ease-of-use for the average Beamer user.

Requires the packages [sfmath](https://ctan.org/pkg/sfmath),
[helvet](https://ctan.org/pkg/helvet) and [PGF/TikZ](https://ctan.org/pkg/pgf)
to be installed in your LaTeX distribution.

Also available as [Overleaf template](https://www.overleaf.com/latex/templates/ugent-beamer/ywtkkxstfgmx).

Demo
----
An extended example is available. See `example/example.tex` and `example/example.pdf` or click [here](https://github.com/driesbenoit/ugent-beamer/blob/master/example/example.pdf).

Some example slides:

![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-0.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-1.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-2.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-3.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-4.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-5.png)
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-6.png)

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

Global installation
-------------------
In case you're using your favorite flavor of Unix (and/or TeX Live) you need to have a local directory (this will probably be ~/texmf/) and you need to place all the files from the theme folder in the directory ~/texmf/tex/latex/beamer/themes/ugent/, finishing it by running texhash.

If on the other hand you're on Windows (probably MiK\TeX) the walkthrough at [this url](http://docs.miktex.org/manual/localadditions.html) explains in detail how to create a local installation. Don't forget to Refresh FNDB as explained [here](http://docs.miktex.org/manual/configuring.html#fndbupdate).

Usage
=====
Refer to the extended example (`example/example.tex`) for an overview of the possibilities of the theme.

Theme options
-------------
The theme options can be set as follows:
`\usetheme[optionshere]{ugent}`

* `language=x`, where x is the language
  * `nl`: dutch (default)
  * `en`: english
* `faculty=x`, where x is the abbreviation of the faculty
  * `lw`: Faculty of Literature & Philosophy
  * `re`: Faculty of Law
  * `we`: Faculty of Science
  * `ge`: Faculty of Medicine and Health Sciences
  * `ea`: Faculty of Engineering and Architecture
  * `eb`: Faculty of Economics and Business Administration
  * `di`: Faculty of Veterinary Medicine
  * `pp`: Faculty of Psychology and Educational Sciences
  * `bw`: Faculty of Bioscience Engineering
  * `fw`: Faculty of Pharmaceutical Sciences
  * `ps`: Faculty of Political and Social Sciences
* `usecolors`
  * This option sets the secondary color equal to the faculty color
  * Always use in combination with `faculty=x`
* `noframenumber`
  * This option suppresses the frame numbers
  
Frame macros
------------
Some frames can be generated automatically:
* `\logoframe`: a white frame with large UGent logo
* `\titleframe`: the title frame
* `\sectionframe`: frame that shows the current section

License
=======
This software is released under the [GNU GPL v3.0 License](https://www.gnu.org/licenses/gpl-3.0.en.html).

Contact
=======
If you are enjoying this theme please share it with your colleagues or friends!

Any suggestions, comments, criticism or appreciation are welcome!
