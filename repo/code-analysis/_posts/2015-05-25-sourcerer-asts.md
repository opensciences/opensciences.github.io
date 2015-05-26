---
title: Sourcerer ASTs
excerpt: "Empirical analysis of the relationship between CC and SLOC in a large corpus of Java methods"
layout: repo-dataset
authors: Davy Landman, Alexander Serebrenik, and Jurgen Vinju
version: 4
---

# URL

* [Data Link (external)](https://repository.cwi.nl/datasets/22454D.tar.xz)
* [Paper in IEEE Xplore Digital Library](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=6976088)

# Change Log

When | What
---- | ----
May 25th, 2015 | Donated by [Davy Landman](maito:davy.landman@gmail.com), Alexander Serebrenik, and Jurgen Vinju.

# Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@INPROCEEDINGS{6976088, 
author={Landman, D. and Serebrenik, A. and Vinju, J.}, 
booktitle={Software Maintenance and Evolution (ICSME), 2014 IEEE International Conference on}, 
title={Empirical Analysis of the Relationship between CC and SLOC in a Large Corpus of Java Methods}, 
year={2014}, 
month={Sept}, 
pages={221-230}, 
keywords={Java;public domain software;software metrics;software quality;source code (software);CC;Java methods;SLOC;cyclomatic complexity;internal source code quality measurement;open-source Java projects;software development;source code quality metric;source lines-of-code;strong linear correlation;Complexity theory;Correlation;Java;Measurement;Software;Transforms;cylcomatic complexity;emperical research;software quality}, 
doi={10.1109/ICSME.2014.44}, 
ISSN={1063-6773},} 
```

# About the Data

## Overview 

Sourcerer is a large corpus of open source Java software. It was constructed by fully downloading the source code of 19 K projects, of which 6 K turned out to be empty. And, after performing the following operations:

 - Remove non-Java files 
 - Remove SCM branches 
 - Remove duplicate projects 
 - Manually reviewed duplicate files  
 - Remove test code

The authors have reduced the 390 GB corpus to 14.3 GB.  The  resulting  corpus  has  been  made  publicly available.

## Paper Abstract

Measuring the internal quality of source code is one of the traditional goals of making software development into an engineering discipline. Cyclomatic Complexity (CC) is an often used source code quality metric, next to Source Lines of Code (SLOC). However, the use of the CC metric is challenged by the repeated claim that CC is redundant with respect to SLOC due to strong linear correlation. We test this claim by studying a corpus of 17.8M methods in 13K open-source Java projects. Our results show that direct linear correlation between SLOC and CC is only moderate, as caused by high variance. We observe that aggregating CC and SLOC over larger units of code improves the correlation, which explains reported results of strong linear correlation in literature. We suggest that the primary cause of correlation is the aggregation. Our conclusion is that there is no strong linear correlation between CC and SLOC of Java methods, so we do not conclude that CC is redundant with SLOC. This conclusion contradicts earlier claims from literature, but concurs with the widely accepted practice of measuring of CC next to SLOC.

