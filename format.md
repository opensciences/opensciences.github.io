---
title: Formatting instructions
layout: journals1
---

## Page Lengths

The Software Science Journal offers review times proportional to
the length of the submission:

+ One month times each  _standard length_.

where _standard length_ is for:

+ Four pages of PDF files, in the format described below,
+ 3400 words of Markdown files (where every figure and table
  counts for 250 words).

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

Note the following required changes to the IEEE styles:

+ No biography entries at the end of the document;
+ No keywords before the start of the article.

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

If your file contains references, then use reference style links
(either _inline_ or otherwise).
Inline:

	An [example](http://url.com/ "Title")

Reference-style labels (titles are optional):

	An [example][id]. Then, anywhere
	else in the doc, define the link:
	
	  [id]: http://example.com/  "Title"





