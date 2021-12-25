***Unofficial uOttawa Thesis LaTeX Template***

**Maintainer:** *Wail Gueaieb*

![GitHub last commit (branch)](https://img.shields.io/github/last-commit/wail-uottawa/uo-thesis/main)
<!-- [![GitHub license](https://img.shields.io/github/license/wail-uottawa/uo-thesis)](https://github.com/wail-uottawa/uo-thesis/blob/master/LICENSE) -->

<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
**Table of Contents**

- [Using the Template](#using-the-template)
    - [Editing Key Fields](#editing-key-fields)
    - [Compilation](#compilation)
    - [Glossary](#glossary)
    - [Graphics](#graphics)
    - [References](#references)
- [Acknowledgment](#acknowledgment)
- [Disclaimer](#disclaimer)

<!-- markdown-toc end -->





# Using the Template

## Editing Key Fields
First, make sure to edit the following key fields at the top of the master file `uo-thesis.tex`: `\thesisauthor`, `\thesistitlecoverpage`, `\thesisdegree`, `\nameofprogram` and `\graduationyear`. 


## Compilation
To process a thesis based on this template, run:  
`pdflatex uo-thesis`	-- first pass of the pdflatex processor  
`bibtex uo-thesis`	-- generates bibliography from .bib data file(s)  
`pdflatex uo-thesis`	-- fixes numbering in cross-references, bibliographic references, glossaries, index, etc.  
`pdflatex uo-thesis`-- fixes numbering in cross-references, bibliographic references, glossaries, index, etc.  
`pdflatex uo-thesis`-- a third time may or may not be necessary, depending on the type of cross-references included in the thesis

By default, the latex output is geared toward generating a PDF version optimized for viewing on an electronic display, including hyperlinks within the PDF.
To create a PDF output that is optimized for double-sided printing:  
1) comment-out the first `\documentclass` statement in the preamble below, and un-comment the second `\documentclass` line.  
2) change the value assigned below to the boolean variable `PrintVersion` from `false` to `true`.


## Glossary
With this template it is easy to include abbreviations, list of symbols, nomenclature, etc. by typing them in the file `glossary.tex` as illustrated in the file. To learn more, please refer to the documentation of the latex package `glossaries-extra`. 


## Graphics
The `pdftex` program allows graphics in the following formats to be
included with the `\includegraphics` command: PNG, PDF, JPEG, TIFF  
Tip 1: Generate your figures and photos in the size you want them to appear
% in your thesis, rather than scaling them with `\includegraphics` options.  
Tip 2: Any drawings you do should be in scalable vector graphic formats:
SVG, PNG, WMF, EPS and then converted to PNG or PDF, so they are scalable in
the final PDF as well. [Inkscape](https://inkscape.org) is a great graphics tool with the ability to generate such formats.   
Tip 3: Photographs should be cropped and compressed so as not to be too large.


## References
Maintaining reference databases can be overwhelming especially for large documents like theses. To that end, it might be a good idea to use a dedicated software to edit and maintain such databases. [JabRef](https://www.jabref.org) is one of the excellent tools for this purpose (among others). 


# Acknowledgment
All the credit goes to the University of Waterloo.
This is mainly a repackaging of their thesis template. 


# Disclaimer
To the best of my knowledge, this template satisfies the current uOttawa thesis [requirements](https://ruor.uottawa.ca/submit-thesis.jsp). However, it is your responsibility to assure that you have met all requirements of the university and your particular department.
