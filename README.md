A Player's Guide to Mathematics
===============================

Write stuff here

Organization and compilation
============================

The book is written with one "chapter" per LaTeX input file.  Each chapter can also be a separate handout given to students; thus each chapter file can also be compiled individually.  A bit of LaTeX wizardry enables both the master file `pgm` and the chapter files to be compiled individually, but requires a bit of help on your part.  If you are on a UNIX-compatible operating system, then run the `lnaux` script.  If you don't want to do this, or if your operating system doesn't support symbolic links, then you can instead add an extra command to your compilation of each chapter file.  E.g. to compile `exploring.tex` you'll need to say

    cp pgm.aux exploring.aux && pdflatex exploring

At some point, it might be worthwhile writing a Makefile that automates the latter.
