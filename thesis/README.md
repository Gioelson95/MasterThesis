# Thesis LaTeX template
This repository is intended to be a collection of suggestions and guidelines to write a thesis.

We (and "we" refers to any right mind person) strongly suggest using LaTeX because it can generate very nice results at the cost of a few code snippets.

In the following, we collect ideas taken from my personal experience, from web pages we trust and from italian [Airlab](http://airwiki.elet.polimi.it/index.php/Tesi) guidelines.

### What is LaTeX
Well, it is a document preparation system.
Basically the writer uses plain text and keyword commands for generating formatted text document.
A well-known guide is [here](http://www.ctan.org/tex-archive/info/lshort/english/lshort.pdf) and you can find help on [WikiBooks](https://en.wikibooks.org/wiki/LaTeX) and [StackExchange](https://tex.stackexchange.com/).
For installation check [here](https://www.latex-project.org/get/).
A nice editor is [texstudio](https://www.texstudio.org/).

The baseline engine is PDFLaTeX, but someone suggests to use LuaLaTeX as it enables very useful packages, especially for graphics and layout control.

### Formats and page layout
You are required to provide a [PDF/A](https://en.wikipedia.org/wiki/PDF/A) file (meant for archiving).
The page layout must be A4, single column, font size 12pt.
We strongly suggest to use serif fonts like Times New Roman, CMU Serif or Latin Modern Roman (the latter is default in latex).
This repository provides you with a `mainA4.tex` template file.
Please read the comments!

### Printed copy
You are NOT asked for a printed copy.
However, it is nice to provide the commission with a hard copy.
In this case, it is relatively straightforward to print the A4 version.
However, the hard copy will be used in a different way with respect to the archive copy.
Therefore it could be better to adjust the page layout and font style.

The [discussion](https://www.nickkolenda.com/font-psychology/) on typefaces is as interesting as old.
Here we report a list of ideas:
- serif fonts are better than sans-serif fonts
- not too condensed, not too tall/short, not too complex
- the option in `\documentclass[twoside]{book}` creates differently sized margin. The logic is the same of "school handbook", enabling the reader to write notes. However we consider it [illogical](https://tex.stackexchange.com/questions/42063/illogical-twoside-margins) and for printing purpose we reverse the margins.
- Someone prefers [B5](https://en.wikipedia.org/wiki/Paper_size#B_series) format instead of A4. Normally the thesis are not longer than 100 pages and therefore a more compact format is confortable. How many A4 books have you read?

Therefore a `mainB5.tex` is provided.
Read its comments!
