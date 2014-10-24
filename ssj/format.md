---
title: Formatting instructions
layout: journal1
---

## Single Page Lengths

The Software Science Journal measures paper size in terms of 
_single lengths_ where such a "single length" is

+ Four pages of PDF files, in the format described below, inclusive of all diagrams, equations and figures.
+ 3400 words of Markdown files (including text of references), where each non-small figure and table
  counts for 250 words. In this context a _small figure_ would be a one line equation rendered as an image.

## Single Lengths and Reviewing

The Software Science Journal offers review times proportional to submission length.

+ One month review cycles for submissions up to _one_ single length;
+ Two month review cycles for submissions up to _two_ single lengths;
+ etc.


## Styles

Papers for the Software Science Journal can be formatted in one
of two ways:

### PDF, IEEE Style

PDF files can be submitted,
generated in  two column format using
the IEEE style files.

For Ms Word, use the double column Word Zip defined
[here](http://www.computer.org/portal/web/peerreviewjournals/author).

For Latex, use the
[style files](http://www.computer.org/portal/web/peerreviewjournals/author).

    \documentclass[journal,10pt]{IEEEtran}

Note: it may be necessary to change the first `\section` heading from

    \IEEEraisesectionheading{\section{Introduction}\label{sec:introduction}}

to

    \section{Introduction}\label{sec:introduction}

Note that SSJ requires the following modifications to the IEEE styles:

+ No biography entries at the end of the document;
+ No keywords before the start of the article.
+ Render bibliographies using the abbrv style (for examples see [here](https://verbosus.com/bibtex-style-examples.html).

### Markdown Files

Our web site can render GitHub-standard Markdown files. To test if your
file uses that style:

+ Create a Github repo;
+ Write your paper as a `X.md` file;
+ Click on the file name in the Github browser and check the formatting.

Note that if your Markdown file contains graphics
(e.g. for equations or especially complex tables)
then those graphics need to be kept in sub-directory
of the directory holding your Markdown in the
directory `img/XXX/` where XXX is some short set of
initials generated from the author names (this will
let us hold your files separately to other authors.

If your file contains references, then use reference style labels:

	An [example][id]. Then, anywhere
	else in the doc, define the link:
	
	  [id]: http://example.com/  "Title"

Note that:

+ The "Title" entry must one one line long and emulate entries in DBLP (see the example below).
+ The URL should point to some publically accessible site that is not maintained by the paper such as the ACM portal
  or IEEE Xplorer. 

For example, here is a reference that links a publications to
the  ACM digital library via a Google shortenner short-cut.

*   _&lbrack;men13a]: http://goo.gl/neqiPD "Tim Menzies: Beyond Data Mining. IEEE Software 30(3): 92 (2013)"_

Note that in-line references such as `[example](http://url.com/ "Title")` should not be used.