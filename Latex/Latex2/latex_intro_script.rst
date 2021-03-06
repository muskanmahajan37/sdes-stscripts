------
Script
------

.. L1

{{{ Show the  first slide containing title, name of the production
team along with the logo of MHRD }}}

.. R1

Hello Friends and welcome to the tutorial on 'Introduction to LaTeX'. 

.. L2

{{{ Show the "Objectives" slide }}}

.. R2

At the end of this tutorial, you will 

1. Get acquainted to LaTeX.
#. Know why we prefer LaTeX?
#. Know the advantages and disadvantages of typesetting documents  
   using the LaTeX approach.
#. Get a brief idea on typical work flow; which uses LaTeX to typeset 
   documents.
#. Know LaTeX commands, LaTeX comments and
   special characters, spacing and actual document content.
#. Be able to create and compile a simple LaTeX document.

.. L3

{{{ Show the "Pre-requisite" slide }}}

.. R3

Before beginning this tutorial, we would suggest having a working installation
of LaTeX on your computer. You can do this by completing the tutorial on 
"LaTeX Installation".

.. L4

{{{ Show the "Introduction" slide }}}

.. R4

LaTeX began as TeX, a computer program originally created by
Donald E. Knuth. It was designed mainly to aid typesetting
of text and mathematical formulae. 

It is a typesetting program that produces excellently typeset documents. 
Typesetting is placing text onto a page with all the style formatting defined,
so that the content looks as intended. It is extensively used for producing 
high quality scientific and mathematical documents. It may also be used for
producing other kinds of documents, ranging from simple one page articles to 
complete books.

LaTeX is pronounced Lah-tech or Lay-tec.
'TeX' is pronounced Tech. 'TeX' is also the first syllable in the Greek word
for technology.

.. L5

{{{ Show the "Why LaTeX?" slide }}}

.. R5

Why we prefer LaTeX?
(a) LaTeX offers excellent visual quality.
(b) Handles typesetting and lets you focus on content.
(c) Makes writing complex Math equation(S) extremely simple.
(d) It is also a standard used widely, especially by the scientific community. 

.. L6

{{{ Show the "Why LaTeX?.." slide }}}

.. R6

We can define LaTex as a document based markup language. This sentence is
deceptively simple, as it reveals a lot about LaTeX. We now break this sentence
up as follows
Mark-up: a system of annotating text, adding extra information to specify 
structure and presentation of text.
Document based markup: you don’t have to worry about each element individually. 

This is essentially a fancy way of saying, LaTeX handles typesetting and lets 
you focus on content rather than appearance.

.. L7

{{{ Show the "Advantages of using  LaTeX" slide }}}

.. R7

Some of the advantages of using LaTeX approach to typesetting are
(1) Easy availability of professionally crafted layouts/templates.
(2) Typesetting of mathematical formulae is supported in a convenient
environment.
(3) Typesetting for most cases can be done with very little learning curve
using easy to use/understand commands, that only specify the logical structure
of the document.
(4) Presence of lots of add-on packages.
(5) It encourages creation of well structured texts.

.. L8

{{{ Show the "Disadvantages of using  LaTeX" slide }}}

.. R8

Some of the disadvantages of using LaTeX approach to typesetting are 
(1) Designing a whole new layout is difficult.
(2) LaTeX is not a word processor, for example, the document author 
is not expected to worry about presentation details like the size of font.

.. L9

{{{ Show the "LaTeX input file format" slide }}}

.. R9

LaTeX input files are simple ASCII text files that are processed by a TeX
processing engine. 
Next comes the question of compiling LaTeX input files and viewing the output
typeset document.
The process is a little different from other markup languages like HTML.
We compile ASCII text files into typeset files that are normally DVI, 
Postscript or PDF files.
The latex command converts LaTeX input files into dvi files.
We can view DVI files on Gnu/Linux using xdvi.
Further,  DVI files can be converted either to a post script file, using the
dvips command or to a PDF file using the dvipdfm command.
The command pdflatex is used to convert LaTeX input files directly to pdf files.
The resultant PDF files can be viewed using standard applications
on most platforms 
(Eg: evince on Gnu/Linux). PDF file are also widely supported.

.. L10

{{{ Show the "Commands,Comments&Special Characters" slide }}}

.. R10

Like most utilities in Linux, LaTeX is case sensitive. Commands begin 
with a backslash. LaTeX environments have a begin and end marker. The begin and
end document commands, mark the beginning and the end of the content of the 
LaTeX document. The text in between the begin and end commands is typeset in 
the output document.Any content after <\end{document}> is ignored. The type of 
document that is being currently typeset in LaTex, is identified with the 
documentclass command. LaTeX then, typesets the document accordingly. 

All the commands in LaTeX begin with a \\. An environment begins with a begin
command and ends with an end command. 

.. L11

{{{ Show the "Commands,Comments&Special Characters.." slide }}}

.. R11

But, how do we write comments with in the document. % character is used
to indicate comments. Anything written after a % symbol in a
line, is ignored.
But what if we wanted to insert the % symbol in the document? We can do so by
escaping it with a \\ (backslash). % is one of the many special characters in
LaTeX. The others are shown on the screen. All of them, except the \\ itself, 
can be inserted by escaping it with a \\. To insert a \\ in our document, 
we use the command \textbackslash.

What would happen if we escape a \\ with a \\? 
A double backslash is actually another command. It inserts a new line in the
typeset document. Normally LaTeX automatically spaces the given input optimally.
But, sometimes we have to insert manual line breaks. The <\\\\>
command or <\newline>
command is used to insert a newline in the output document. A 
single line break in the input document, doesn't cause any change in the 
output document.

A single empty line causes a change in paragraphs in the output. Multiple 
empty lines are equivalent to a single empty line. Similarly, multiple spaces
are treated as a single space.

.. L12

{{{ Show the "Typesetting a minimal document" slide }}}

.. R12

Now, try to create a simple LaTeX document. Pause the tutorial and type the
content shown on the screen in a text editor. Save the file as temp.tex

.. L13

{{{continue from paused state}}}
{{{ Show the "Compiling to DVI & PDF" slide }}}

.. R13

Now we compile the commands in the LaTeX input file that is, temp.tex into a 
typeset file. 

The first alternative is to compile LaTeX input file into a DVI 
file. We use the latex command for this purpose. For compiling the LaTeX input 
file temp.tex into a DVI file, we use the following command

<latex temp.tex>

The output file would be temp.dvi.

The other alternative is to create PDF files from LaTeX input files.
We use the pdflatex command for this purpose. For compiling the LaTeX input
file temp.tex into a PDF file, we use the following command

<pdflatex temp.tex>

Please note that, throughout this course we shall be using pdflatex to compile 
our documents.

.. L14

{{{ Show the "Summary" slide }}}
    
.. R14

This brings us to the end of this tutorial. In this tutorial, we have learnt

1. About LaTeX.
#. Why we prefer LaTeX.
#. The advantages and disadvantages of typesetting documents  
   using the LaTeX approach.

.. L15

{{{ Show the "Summary.." slide }}}

.. R15

This brings us to the end of this tutorial. In this tutorial, we have learnt

#. A description, of a typical work flow; which uses LaTeX to typeset 
   documents.
#. The ability to recognize and differentiate between LaTeX commands, LaTeX
   comments and special characters, spacing and actual document content.
#. To Create and compile a simple LaTeX document.


.. L16

{{{ Show the "Self assessment questions" slide }}}

.. R16

Here are some self assessment questions for you to solve

 1. Convert the temp.dvi created during the course of this tutorial to 
    temp_1.ps using the dvips command. Verify that the two files 
    indeed look the same.

 2. Convert the temp.dvi created during the course of this tutorial to
temp_1.pdf using the dvipdfm command. Verify that the two files indeed look the
same.

.. L17

{{{ Show the "Solutions" slide }}}

.. R17

And the answers,

1. dvips -o temp_1.ps temp.dvi

2. dvipdfm -o temp_1.pdf temp.dvi

.. L18

{{{ Show the SDES & FOSSEE slide }}}

.. R18

Software Development techniques for Engineers and Scientists - SDES, is an 
initiative by FOSSEE. For more information, please visit the given link.

Free and Open-source Software for Science and Engineering Education - FOSSEE, is
based at IIT Bombay which is funded by MHRD as part of National Mission on 
Education through ICT.

.. L19

{{{ Show the ``About the Spoken Tutorial Project'' slide }}}

.. R19

Watch the video available at the following link. It summarises the Spoken 
Tutorial project.If you do not have good bandwidth, you can download and 
watch it. 

.. L20

{{{ Show the `` Spoken Tutorial Workshops'' slide }}}

.. R20

The Spoken Tutorial Project Team conducts workshops using spoken tutorials,
gives certificates to those who pass an online test.

For more details, contact contact@spoken-tutorial.org

.. L21

{{{ Show the Acknowledgements slide }}}

.. R21

Spoken Tutorial Project is a part of the "Talk to a Teacher" project.
It is supported by the National Mission on Education through ICT, MHRD, 
Government of India. More information on this mission is available at the 
given link.

.. L22

{{{ Show the Thankyou slide }}}

.. R22

Hope you have enjoyed this tutorial and found it useful.
Thank you!
