=== LaTeX Style for Glasgow University Thesis ===
LaTeX style template for Glasgow theses.

== Required LaTeX Packages ==
All of these are distributed with TeXlive/MikTeX
* times
* setspace
* parskip
* titlesec
* geometry


== Optional Packages ==
All of these are distributed with TeXlive/MikTeX and are highly recommended
* biblatex
* csquotes
* babel
* inputenc
* verbatim
* biblatex-chicago (for citations using Chicago Manual of Style)

If you are using Debian/Ubuntu, all but biblatex-chicago are packaged in: texlive-latex-base, texlive-latex-recommended, and texlive-latex-extra

== Usage ==
\documentclass[a4paper,12pt]{report} % feel free to use with different document classes
\usepackage{glasgow-thesis} % load this style.
\title{Thesis Title}
\author{James Ross} % your name
\qualifications{M.A, University of Glasgow \\ B.A., University of Glasgow} % your current qualifications, separated by \\ (newline)
\degree{Doctor of Philosophy} % degree for which this thesis is being submitted
\school{Engineering} % school within university
\college{Sciences} % college within university
\date{September 2011} % month and year in which thesis is deposited
\begin{document}
	\pagenumbering{roman}
	\maketitle
	\begin{abstract}
		abstract
	\end{abstract}
	\tableofcontents
	\clearpage
	\setcounter{page}{0}
	\pagenumbering{arabic}
	% thesis begins here
\end{document}
