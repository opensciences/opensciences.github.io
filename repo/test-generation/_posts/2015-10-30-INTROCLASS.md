---
title: INTROCLASS dataset
excerpt: "Is the Cure Worse Than the Disease? Overfitting in Automated Program Repair"
layout: repo-dataset
authors: "Edward K. Smith, Earl T. Barr, Claire Le Goues, Yuriy Brun"
version: 4
---

# URL

* [Data Link (DOI)](https://doi.org/10.5281/zenodo.581789)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2786825&dl=ACM)

# Change Log

When | What
---- | ----
October 30th, 2015 | Donated by [Edward K. Smith](mailto: tedks@cs.umass.edu)

# Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{Smith:2015:CWD:2786805.2786825,
 author = {Smith, Edward K. and Barr, Earl T. and Le Goues, Claire and Brun, Yuriy},
 title = {Is the Cure Worse Than the Disease? Overfitting in Automated Program Repair},
 booktitle = {Proceedings of the 2015 10th Joint Meeting on Foundations of Software Engineering},
 series = {ESEC/FSE 2015},
 year = {2015},
 isbn = {978-1-4503-3675-8},
 location = {Bergamo, Italy},
 pages = {532--543},
 numpages = {12},
 url = {http://doi.acm.org/10.1145/2786805.2786825},
 doi = {10.1145/2786805.2786825},
 acmid = {2786825},
 publisher = {ACM},
 address = {New York, NY, USA},
 keywords = {GenProg, IntroClass, TrpAutoRepair, automated program repair, empirical evaluation, independent evaluation},
}
```

# About the Data

## Overview of Data

The INTROCLASS dataset of 998 bugs in versions of six small C programs, together with two types of tests and human-written bug fixes. The dataset is drawn from an introductory C programming class at UC Davis with an enrollment of about 200 students. The use of this anonymized dataset for research was approved by the UC Davis IRB. To prevent identity recovery, students’ names in the dataset 998 of the 778 black box and 845 white box buggy versions are unique.

## Attribute Information

program , LOC, tests, buggy versions, computation

## Paper Abstract

Automated program repair has shown promise for reducing the significant manual effort debugging requires. This paper addresses a deficit of earlier evaluations of automated repair techniques caused by repairing programs and evaluating generated patches' correctness using the same set of tests. Since tests are an imperfect metric of program correctness, evaluations of this type do not discriminate between correct patches and patches that overfit the available tests and break untested but desired functionality. This paper evaluates two well-studied repair tools, GenProg and TrpAutoRepair, on a publicly available benchmark of bugs, each with a human-written patch. By evaluating patches using tests independent from those used during repair, we find that the tools are unlikely to improve the proportion of independent tests passed, and that the quality of the patches is proportional to the coverage of the test suite used during repair. For programs that pass most tests, the tools are as likely to break tests as to fix them. However, novice developers also overfit, and automated repair performs no worse than these developers. In addition to overfitting, we measure the effects of test suite coverage, test suite provenance, and starting program quality, as well as the difference in quality between novice-developer-written and tool-generated patches when quality is assessed with a test suite independent from the one used for patch generation.
