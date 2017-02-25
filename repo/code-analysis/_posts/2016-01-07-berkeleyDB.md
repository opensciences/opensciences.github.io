---
title: BerkeleyDB
excerpt: "Language-Independent, Automated Software Composition"
layout: repo-dataset
authors: "Sven Apel, Christian Kastner, Christian Lengauer"
version: 4
---

# URL

* [Data Link (DOI)](https://doi.org/10.5281/zenodo.268483)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=1555038)

# Change Log

When | What
---- | ----
November 2nd, 2015 | Donated by [Sven Apel](mailto:apel@uni-passau.de)

# Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{Apel:2009:FLA:1555001.1555038,
 author = {Apel, Sven and Kastner, Christian and Lengauer, Christian},
 title = {FEATUREHOUSE: Language-independent, Automated Software Composition},
 booktitle = {Proceedings of the 31st International Conference on Software Engineering},
 series = {ICSE '09},
 year = {2009},
 isbn = {978-1-4244-3453-4},
 pages = {221--231},
 numpages = {11},
 url = {http://dx.doi.org/10.1109/ICSE.2009.5070523},
 doi = {10.1109/ICSE.2009.5070523},
 acmid = {1555038},
 publisher = {IEEE Computer Society},
 address = {Washington, DC, USA},
}
```

# About the Data

## Overview of Data

Berkeley DB is Oracle’s Embedded Storage Engine. The data contains its source code which has been applied to FEATUREHOUSE

## Paper Abstract

Superimposition is a composition technique that has been applied successfully in many areas of software development. Although superimposition is a general-purpose concept, it has been (re)invented and implemented individually for various kinds of software artifacts. We unify languages and tools that rely on superimposition by using the language-independent model of feature structure trees (FSTs). On the basis of the FST model, we propose a general approach to the composition of software artifacts written in different languages, Furthermore, we offer a supporting framework and tool chain, called FEATUREHOUSE. We use attribute grammars to automate the integration of additional languages, in particular, we have integrated Java, C#, C, Haskell, JavaCC, and XML. Several case studies demonstrate the practicality and scalability of our approach and reveal insights into the properties a language must have in order to be ready for superimposition.
