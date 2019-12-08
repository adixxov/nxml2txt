nxml2txt
========

Distributional Semantics Resources for Biomedical Text Processing
Sampo Pyysalo1 Filip Ginter2 Hans Moen3 Tapio Salakoski2 Sophia Ananiadou1
1. National Centre for Text Mining and School of Computer Science
University of Manchester, UK
2. Department of Information Technology
University of Turku, Finland
3. Department of Computer and Information Science
Norwegian University of Science and Technology, Norway
sampo@pyysalo.net ginter@cs.utu.fi hans.moen@idi.ntnu.no
tapio.salakoski@utu.fi sophia.ananiadou@manchester.ac.uk
========

NLM .nxml to text format conversion 

Usage:

    ./nxml2txt NXMLFILE [TEXTFILE] [SOFILE]

For example (using test document):

    ./nxml2txt test/PMC3357053.nxml test/PMC3357053.txt test/PMC3357053.so

This creates the files `test/PMC3357053.txt`, containing the text
content of the input document, and `test/PMC3357053.so`, containing
the annotations (XML elements and their attributes) in a simple
standoff format.

nxml2txt assumes a unix-like environment.
If the input .nxml file contains embedded TeX-math, nxml2txt
requires [LaTeX](http://en.wikipedia.org/wiki/LaTeX) and
[catdvi](http://catdvi.sourceforge.net/).

This tool was originally introduced as part of the BioNLP Shared Task
2011 supporting resources
(https://github.com/ninjin/bionlp_st_2011_supporting).
