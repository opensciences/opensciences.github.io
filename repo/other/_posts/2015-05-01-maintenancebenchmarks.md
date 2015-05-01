---
title: maintenancebenchmarks
excerpt: "A dataset from change history to support evaluation of software maintenance tasks"
layout: repo
authors: "Bogdan Dit; Andrew Holtzhauer; Denys Poshyvanyk; Huzefa Kagdi"
version: 4
---

#URL

* [Data in Terapromise](https://terapromise.csc.ncsu.edu:8443/!/#repo/view/head/other/maintenancebenchmarks)
* [Paper in IEEE Explore](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=6624019)

#Change Log

When | What
---- | ----
May 1st, 2015| Donated by [Bogdan Dit](/repo/people/data-donors/promise4.html)

#Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@INPROCEEDINGS{6624019, 
author={Dit, B. and Holtzhauer, A. and Poshyvanyk, D. and Kagdi, H.}, 
booktitle={Mining Software Repositories (MSR), 2013 10th IEEE Working Conference on}, 
title={A dataset from change history to support evaluation of software maintenance tasks}, 
year={2013}, 
month={May}, 
pages={131-134}, 
keywords={Java;software maintenance;Java applications;SE tasks;change history;change request textual description;feature location;impact analysis;software engineering tasks;software maintenance tasks;source code;Benchmark testing;Gold;Java;Large scale integration;Software maintenance;Software systems;Generate Benchmarks;datasets;feature location;impact analysis}, 
doi={10.1109/MSR.2013.6624019}, 
ISSN={2160-1852},}
```

#About the Data

##Overview of Data

This dataset contains two new datasets for ArgoUML0.24 and ArgoUML0.26.2, as well as a suite of Java tools used to generate these benchmarks, and two Matlab scripts that use VSM and LSI to compute the similarities between a query and the methods of a system (i.e., the corpus).

##Attribute Information

### Traces Format

The format of a JPDA trace is as following:

```
thread name  Number of pipes ("|") denote call stack depth methodName  --  ClassNameWithFullPath$InnerClass
```

Example:

```
main:0:| 5:2  processOptions  --  org.mozilla.javascript.tools.shell.Main
main:0:| 5:2  init  --  org.mozilla.javascript.tools.shell.Global
main:0:| | 5:2  <init>  --  org.mozilla.javascript.tools.shell.Global$1
main:0:| | 5:2  call  --  org.mozilla.javascript.ContextFactory
main:0:| | 5:2  call  --  org.mozilla.javascript.ContextFactory
main:0:| | 5:2  <init>  --  org.mozilla.javascript.ScriptableObject$Slot
main:0:| | | 5:2  <clinit>  --  org.mozilla.javascript.Context
main:0:| | | | 5:2  <clinit>  --  org.mozilla.javascript.ScriptRuntime
main:0:| | | | | 5:2  classOrNull  --  org.mozilla.javascript.Kit
```

Remarks

 * `$1` denotes an anonymous class
 * `<init>` is the class constructor, and should be replaced with the actual name of the class (e.g., from org.mozilla.javascript.tools.shell.Global.<init> to org.mozilla.javascript.tools.shell.Global.Global)
 * `<clinit>` is for static block or class initialization (can be discarded)
 * the trace does not capture the signature of the methods

##Paper Abstract

Approaches that support software maintenance need to be evaluated and compared against existing ones, in order to demonstrate their usefulness in practice. However, oftentimes the lack of well-established sets of benchmarks leads to situations where these approaches are evaluated using different datasets, which results in biased comparisons. In this data paper we describe and make publicly available a set of benchmarks from six Java applications, which can be used in the evaluation of various software engineering (SE) tasks, such as feature location and impact analysis. These datasets consist of textual description of change requests, the locations in the source code where they were implemented, and execution traces. Four of the benchmarks were already used in several SE research papers, and two of them are new. In addition, we describe in detail the methodology used for generating these benchmarks and provide a suite of tools in order to encourage other researchers to validate our datasets and generate new benchmarks for other subject software systems. Our online appendix: [http://www.cs.wm.edu/semeru/data/msr13/](http://www.cs.wm.edu/semeru/data/msr13/).
