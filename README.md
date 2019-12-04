# GMPL Syntax Highlighting

Scope of this project is to enable syntax highlighting for the [GNU MathProg optimization modeling language](https://en.wikibooks.org/wiki/GLPK/GMPL_%28MathProg%29) 
(previously known as GMPL) for the [GLPK (GNU Linear Programming Kit)](https://www.gnu.org/software/glpk/) in some popular open source text editors, in particular

* [GNOME's gedit](https://gitlab.gnome.org/GNOME/gedit/), which comes with the GNOME desktop environment, e.g. in Ubuntu
* [Notepad++](https://notepad-plus-plus.org/), which is a very popular text editor for Windows


## Introduction
The [GNU MathProg modeling language](https://www.gnu.org/software/glpk/), also known as GMPL, is a powerful algebraic modeling language (AML) to formulate linear and mixed integer linear optimization problems. Its syntax strongly resembles that of the well-known algebraic modeling language [AMPL](https://ampl.com/). GNU MathProg is part of the [GNU Linear Programming Kit (GLPK)](https://www.gnu.org/software/glpk/) and is supported by the standalone solver of GPLK, that is GLPSOL. GPLK and GNU MathProg are readily available on most Linux systems, in particular in the official package repositories of Ubuntu, Debian, Raspian and installable via `apt install glpk-utils`. 

I often use GMPL as a prototyping tool to try out different formulations for optimization problems on static data, before I go for more software development friendly optimization modeling languages like e.g. [Pyomo in Python](http://www.pyomo.org/) with its object-oriented modeling capabilities. 

However, I found that at least under the versatile [GNOME's gedit](https://wiki.gnome.org/Apps/Gedit) there is no syntax highlighting for this very helpful AML. The same holds for the widespread open source editor [Notepad++](https://notepad-plus-plus.org/) for Windows. This is why I took the liberty of writing syntax highlighting definitions for the GNU MathProg language for both gedit and Notepad++. Both syntax definitions are published as open source under the [GNU General Public License Version 2 (GPLv2)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html) in analogy to the aforementioned editors. 

Note that this is open source software. As stated in the GPLv2, this software comes without any warranty and any usage is completely at your own risk. 


## How to use the language definitions
For detailed instructions on how to include the language definition files for GNU MathProg into both gedit and Notepad++ see the [instructions in my blog philippstelzig.de/blog](https://philippstelzig.de/blog/gnu-mathprog-in-gedit-and-notepad/). 

Roughly speaking, the procedure is as follows. 

### gedit
The official GNOME documentation offers [instructions on how to include new language definitions into gedit](https://developer.gnome.org/gtksourceview/stable/lang-reference.html). 


### Notepad++
The Notepad++ editor offers the definition, import and export of user-defined languages (UDL). Open Notepad++, in the menu bar click Language/Define your language..., then import the `gmpl.xml` from the repository. 


# Authors
The syntax higlighting definitions for GMPL have been developed by the following authors:
* [Dr. Philipp Emanuel Stelzig](mailto:software@philippstelzig.de)


# Special Thanks
Special thanks to [Dr. Harald Held](https://gitlab.com/harald.held) for finding bugs and trying out the highlighting definition!
