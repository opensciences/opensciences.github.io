---
title: Call Graphs for Javascript IDEs
excerpt: "Efficient Construction of Approximate Call Graphs for JavaScript IDE Services"
layout: repo-dataset
authors: "Asger Feldthaus, Max Schäfer, Manu Sridharan, Julian Dolby Frank Tip"
version: 4
---

# URL

* [Data in Terapromise](https://terapromise.csc.ncsu.edu:8443/!/#repo/view/head/other/mozillaanthropology)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?doid=2635868.2635887)

# Authors
* [Asger Feldthaus, Max Schäfer, Manu Sridharan, Julian Dolby, and Frank Tip](mailto: asf@cs.au.dk,schaefer@ntu.edu.sg,msridhar@us.ibm.com,dolby@us.ibm.com,ftip@uwaterloo.ca)

# Change Log

When | What
---- | ----
May 1st, 2015 | Donated by [Asger Feldthaus](mailto:asf@cs.au.dk)

# Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{feldthaus2013efficient,
  title={Efficient construction of approximate call graphs for JavaScript IDE services},
  author={Feldthaus, Asger and Schafer, Markus and Sridharan, Manu and Dolby, Julian and Tip, Frank},
  booktitle={Software Engineering (ICSE), 2013 35th International Conference on},
  pages={752--761},
  year={2013},
  organization={IEEE}
}
```

# About the Data

## Overview of Data

The authors have run their algorithms on ten real-world  subject  programs  and  measured their performance. The programs include  medium  to  large browser-based  JavaScript  applications  covering  a  number  of different domains, including games (beslimed,pacman,pong), visualizations  (3dmodel,coolclock),  editors (htmledit,mark-itup), a presentation library (flotr), a calendar app (fullcalen-dar), and a PDF viewer (pdfjs).

## Paper Abstract

The rapid rise of JavaScript as one of the most popular programming languages of the present day has led to a demand for sophisticated IDE support similar to what is available for Java or C#. However, advanced tooling is hampered by the dynamic nature of the language, which makes any form of static analysis very difficult. We single out efficient call graph construction as a key problem to be solved in order to improve development tools for JavaScript. To address this problem, we present a scalable field-based flow analysis for constructing call graphs. Our evaluation on large real-world programs shows that the analysis, while in principle unsound, produces highly accurate call graphs in practice. Previous analyses do not scale to these programs, but our analysis handles them in a matter of seconds, thus proving its suitability for use in an interactive setting.
