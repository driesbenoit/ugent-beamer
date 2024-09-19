# Version v1.0
The aim of this UGent Beamer theme:
* A theme that closely resembles the official UGent Powerpoint/Keynote presentation themes.
* Similar theme options as the [depreciated UGent Beamer theme](https://github.com/pbelmans/ugent-beamer) by Pieter Belmans.
* A corporate version, as well as faculty specific versions.
* Ease-of-use for the average Beamer user.

Requires the packages [sfmath](https://ctan.org/pkg/sfmath),
[helvet](https://ctan.org/pkg/helvet) and [PGF/TikZ](https://ctan.org/pkg/pgf)
to be installed in your LaTeX distribution (which most likely is already the case, see below).

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
![](https://github.com/driesbenoit/ugent-beamer/blob/master/example-screenshots/screenshot-7.png)

Download
========
Download the latest release by following [this](https://github.com/driesbenoit/ugent-beamer/releases) link.

Installation
============
The theme is an addendum for the LaTeX beamer class, hence it is assumed that you have a running LaTeX installation together with the beamer package and its dependencies.

Once you have the files, all that is required for the theme to work is putting the files into a directory where LaTeX can find them. This boils down to mimicking the so called TDS (or TeX Directory Structure).

Ad-hoc installation 
-------------------
After downloading, copy the files named beamer*ugent.sty, together with all files in the image folder, into the same folder as your LaTeX source file.

Then include the theme by writing:
```latex
\documentclass{beamer}

\usetheme{ugent}
```
in the preamble of your document.

Global installation
-------------------
In case you're using your favorite flavor of Unix (and/or TeX Live) you need to have a local directory (this will probably be `~/texmf/`) and you need to place all the files from the theme folder in the directory `~/texmf/tex/latex/beamer/themes/ugent/`, finishing it by running texhash (however, running texhash is no longer necessary for recent Tex Live versions).

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
* `logoa=x`, where x is the name of a logofile 
  * The logo's of some frequent UGent partners are packaged with the theme.
  * These include: `fwo`,`flandersmake`,`imec`,`vito`,`vib` and `vlaio`.
  * Users can provide any logo and included it with `logoa=mylogo`. Of course, `mylogo` should then be made available to the compiler, e.g. via the image folder of the presentation. The *right* amount of whitespace around the logo will align it nicely with the UGent logo.
* `logob=x`, where x is the name of a logofile 
  * See `logoa=x`.
  * Only takes effect when `logoa=x` is also set.
* `logoc=x`, where x is the name of a logofile 
  * See `logoa=x`.
  * Only takes effect when `logob=x` is also set.
* `seccolor=x`, where x is the name of a color
  * This option overrides the default secondary color (which is ugentyellow for the corporate theme or, if the faculty option is set, the faculty color).
  * Color names could be any color known by `xcolor`, e.g. green, lightblue, etc. 
  * Also faculty color names can be used, e.g. ugent-ge, ugent-di, etc.
  * Note that this option and behavior makes the option `usefacultycolors`, available in older versions of the theme, obsolete.
* `noframenumber`
  * This option suppresses the frame numbers
  
Frame macros
------------
Some frames can be generated automatically:
* `\logoframe`: a white frame with large UGent logo
* `\titleframe`: the title frame
* `\sectionframe`: frame that shows the current section

Closingframe
------------
A special frame environment is available to create a closing slide. 
The environment creates a frame with the same background as the titleframe.
Text and images should be inserted via `itemize` environments in order to be rendered correctly.
The minimal syntax is:
```
\begin{closingframe}
    \begin{itemize}
        \item Some text 
        \item More text 
    \end{itemize}
\end{closingframe}
```
For an extended example of the closingframe, see the last screenshot above and the syntax in the examples.

License
=======
This software is released under the [GNU GPL v3.0 License](https://www.gnu.org/licenses/gpl-3.0.en.html).

Contact
=======
If you are enjoying this theme please share it with your colleagues or friends!

Any suggestions, comments, criticism or appreciation are welcome!
