.. Objectives
.. ----------

.. By the end of this tutorial, you will be able to

.. 1. Understand basic structure of a LaTeX document, its various document
..    classes and loading packages that add new features to the LaTeX system.
.. #. Create a LaTeX document with a title and an abstract.
.. #. Create numbered and non-numbered sections and subsections in a LaTeX
..    document.
.. #. Create an appendix in a LaTeX document.
.. #. Create a table of content in a LaTeX document.

.. Prerequisites
.. -------------

.. 1. latex_intro 

     
.. Author              : Harish Badrinath < harish [at] fossee [dot] in > 
   Internal Reviewer   : 
   External Reviewer   :
   Langauge Reviewer   : 
   Checklist OK?       : <put date stamp here, if OK> 

Script
------

.. L1

{{{ Show the  first slide containing title, name of the production
team along with the logo of MHRD }}}

.. R1

Hello friends and welcome to the tutorial on Basics of LaTeX and its document
structure.

.. L2

{{{ Show the objectives slide }}}

.. R2

.. By the end of this tutorial, you will be able to

.. 1. Understand basic structure of a LaTeX document, its various document
..    classes and loading packages that add new features to the LaTeX system.
.. #. Create a LaTeX document with a title and an abstract.
.. #. Create numbered and non-numbered sections and subsections in a LaTeX
..    document.
.. #. Create an appendix in a LaTeX document.
.. #. Create a table of content in a LaTeX document.

.. L3

{{{ Switch to the pre-requisite slide }}}

.. R3

Before beginning this tutorial,we would suggest having a working installation of
LaTeX and suggest you to complete the tutorial titled "Introduction to LaTeX".

.. L4

{{{ Basic Structure of a LaTeX document }}}
\documentclass{article}
\begin{document}
SAMPLE TEXT
\end{document}

.. R4

the text "SAMPLE TEXT" is illustrative and can be replaced replaced by a 
single alpha-numeric character, for example. When done so, the resulting 
document could be described as the shortest possible LaTeX input document, that
creates an output file. It consists of 3 LaTeX commands and one line/character
of text.
This is processed by a TeX processor that generates an output file. Now, we 
begin to look into each line in the example in more detail.
The first line reads

.. L5

\documentclass{article}

.. R5

which more generally can be written as

.. L6

\documentclass [parameters] {DocumentClass}

.. R6

Where \documentclass is a LaTeX command.
Parameters specify if you want to use a non default font size, for example.
More specifically the parameters can be used to alter things like font size of 
the document, paper size, two sided or single sided printing, etc.

.. L7

\documentclass[12pt,a4paper,draft]{report} 

.. R7

This command instructs LaTeX to 
Create a new document of class report. The available classes are article, proc,
report, book, slides, letter.
12 pt: sets the font size of main font. Other are relatively adjusted. 10pt is
the default. 
a4paper: specifies the paper size
draft:  marks hyphenation and justification problems in typesetting
with a square in the margin

.. L8

\usepackage[options]{...}

.. R8

This statement can be used optionally and is used to include packages, which are
used to extend the LaTeX's capabilities. There are a number of packages that are
included by default with LaTeX2 base distribution. You can use the texdoc
command for accessing package documentation.

.. L9
::

\documentclass{article}
\title{My First LaTeX Document}
\author{Harish}
\date
\begin{document}
Hello world!
\end{document}

.. R9

We add the LaTeX commands, that specify the title and the author of the
document. When we compile the document shown to an output file and view it we
notice that output is, as seen no different from not adding the fields of title
and author. We need to add another command to actually show the title author 
and date in the output document. We add the command in the following example.

.. L10

\documentclass{article}
\title{My First LaTeX Document}
\author{Harish}
\begin{document}
\maketitle
Hello world!
\end{document}

.. R10

The command \maketitle adds title, authors name and date to the output file.
Of these only the date is optional. If date command is specified, then the given
date is used else today's date is used. 

.. L11

\documentclass{article}
\title{My First LaTeX Document}
\author{Harish}
\begin{document}
\maketitle
Hello world!
\begin{abstract}
An Example Abstract
\end{abstract}
\end{document}

.. R11

The abstract command is used to insert abstract of a document, into the output
file.Place it in the location, where you want your abstract to present in
the document. It is available for the document classes article and report, but
not book

.. L12

\documentclass{article}
\title{My First LaTeX Document}
\author{Harish}
\begin{document}
\maketitle
Hello world!
\begin{abstract}
An Example Abstract
\end{abstract}
\section{Numbered Section 1}
Section1 Text
\section{Numbered Section 2}
Section2 Text
\section*{Unnumbered Section 1}
Section3 Text
\section*{Unnumbered Section 2}
Section4 Text
\end{document}


.. R12

Titles chapters and sections are used to help the user find his or her way
through your work. The following commands are available in the article class:
section, subsection, subsubsection,  paragraph and sub paragraph. The default
behavior is to use numbered sections. We can use un-numbered sections appending
* to section command. If you want to split your document without influencing the
section or chapter numbering use the part command.

.. L13

\documentclass{book}
\title{My first Book}
\author{Harish}
\date{31-February-2012}
\begin{document}
\maketitle
\chapter{My First Chapter}
Main
\section{Section1}
Section 1 Text
\subsubsection{My First Subsection}
Numbered-Section 1's Subsection Text
\section{Section2}
Numbered-Section 2 Text
\section*{Section3}
First un-numbered Section Text
\section*{Section4}
Second un-numbered Section Text
\chapter{So We say goodbye}
Thank you for reading dear reader
\end{document}

.. R13

Longer documents can use report or book class. We can add a new chapter using
the chapter command, provided by the report or book class. After compiling the
file shown in the slide we notice that subsections are not numbered. 

.. L14

\setcounter{secnumdepth}{3}

.. R14
We can change this behavior with the command setcounter , calling it as shown
in the slide. 

.. L15

\appendix

.. R15

Appendix can be added to the document using \appendix command. any content after
\appendix will be added to the appendix. In the report or book class, we have to
use \chapter to indicate that the chapters are to be numbered as appendices.

similarly for the article class we have to use the section command to indicate
that sections are to be numbered as appendices.

.. L16


.. R16

Lets add a Table of content to the document. The LaTeX command to add a TOC to a
document is using \tableofcontents command. It is used at the point at which the
table of content is to be placed. You then have to compile the input file twice
to produce a text. 
Any numbered section/chapter appear automatically in the table of content.

.. L17


.. R17

Un-numbered sections are added to TOC using \addcontentsline command.
For example we use the command
\addcontentsline{toc}{section}{Intro}
where intro is the text that you want to appear in the Table of contents.

.. L18

{{{ Show summary slide }}}

.. R18

This brings us to the end of this tutorial. In this tutorial, we have,

.. 1. Gained an understanding of the basic structure of a LaTeX document, its 
..    various document classes and loading packages that add new features to 
..    the LaTeX system.
.. #. Created a LaTeX document with a title and an abstract.
.. #. Created both numbered and non-numbered sections and subsections in a 
..    LaTeX document.
.. #. Created an appendix in a LaTeX document.
.. #. Created a table of content in a LaTeX document.

.. L19

{{{Show self assessment questions slide}}}

.. R19

Here are some self assessment questions for you to solve

 1. Is the LaTeX code given below a valid input file (File compiles successfully
and produces the intended result, that is to produce a book with two chapters 
and an appendix.
\begin{verbatim}
\documentclass{book}
\title{My first Book}
\author{Harish}
\date{31-February-2012}
\begin{document}
\maketitle
\chapter{My First Chapter}
Main
\chapter{So We say goodbye}
Thank you for reading dear reader
\appendix
\section{First Appendix}
\end{document}
\end{verbatim}

 2. Does making the subsections placed at any arbitrary level, get numbered by
default using the appropriate setcounter command  with secnumdepth parameter
make the subsections appear automatically in the table of content ??

.. L20

{{{Show self assessment questions slide}}}

.. R20

And the answers,

1. Although the given file looks syntactically valid, the output file is not what
we expected. This is mainly because we are trying to use the section command to
create sections in the appendix, for a document whose type is given as a book.

2. No The \tableofcontents command normally shows only numbered section
headings, and only down to the level defined by the tocdepth counter.

.. L21

{{{ Show the thankyou slide }}}

.. R21

Hope you have enjoyed this tutorial and found it useful.
Thank you!