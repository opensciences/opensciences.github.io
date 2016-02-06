---
title: bugclassify
excerpt: "It’s Not a Bug, It’s a Feature: Does Misclassification Affect Bug Localization?"
layout: repo-dataset
authors: "Pavneet Singh Kochhar; Tien-Duy B. Le; David Lo"
version: 4
---


# URL

* [Data in Terapromise](https://terapromise.csc.ncsu.edu:8443/svn/repo/other/bugclassify)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2597105)

# Change Log

When | What
---- | ----
March 13, 2015 | Donated by [Pavneet Singh Kochhar](/repo/people/data-donors/promise4.html)


# Reference

Studies who have been using the data (in any form) are required to add the following reference to their report/paper:

```
@inproceedings{Kochhar:2014:BFM:2597073.2597105,
 author = {Kochhar, Pavneet Singh and Le, Tien-Duy B. and Lo, David},
 title = {It's Not a Bug, It's a Feature: Does Misclassification Affect Bug Localization?},
 booktitle = {Proceedings of the 11th Working Conference on Mining Software Repositories},
 series = {MSR 2014},
 year = {2014},
 isbn = {978-1-4503-2863-0},
 location = {Hyderabad, India},
 pages = {296--299},
 numpages = {4},
 url = {http://doi.acm.org/10.1145/2597073.2597105},
 doi = {10.1145/2597073.2597105},
 acmid = {2597105},
 publisher = {ACM},
 address = {New York, NY, USA},
 keywords = {Bug Localization, Misclassification},
}
```

# About the Data

They download Herzig et al.'s datasets which included the identiers of issue reports that they have manually analyzed. The description of that dataset follows.

The authors conducted a study on five open-source JAVA projects described in Table I (see paper). They aimed to select projects that were under active development and were developed by teams that follow strict commit and bug fixing procedures similar to industry. They also aimed to have a more or less homogenous data set which eased the manual inspection phase. Projects from APACHE and MOZILLA seemed to fit their requirements best. Additionally, they selected the five projects such that they cover atleast two different and popular bug tracking systems: Bugzilla1 and Jira2. Three out of five projects (Lucene-Java, Jackrabbit,and HTTPClient) use a Jira bug tracker. The remaining two projects (Rhino, Tomcat5) use a Bugzilla tracker. For each of the five projects, they selected all issue reports that were marked as being RESOLVED , CLOSED, or VERIFIED and whose resolution was set to FIXED and performed a manual inspection on these issues. They disregarded issues with resolution in progress or not being accepted, as their features may change in the future.The number of inspected reports per project can be found in the table above. In total, they obtained 7,401 closed and fixed issue reports. 1,810 of these reports originate from the Rhino and Tomcat5 projects and represent Bugzilla issue reports. The remaining of the 5,591 reports were filed in a Jira bug tracker.


## Abstract

Bug localization refers to the task of automatically process- ing bug reports to locate source code files that are respon- sible for the bugs. Many bug localization techniques have been proposed in the literature. These techniques are often evaluated on issue reports that are marked as bugs by their reporters in issue tracking systems. However, recent findings by Herzig et al. find that a substantial number of issue re- ports marked as bugs, are not bugs but other kinds of issues like refactorings, request for enhancement, documentation changes, test case creation, and so on. Herzig et al. report that these misclassifications affect bug prediction, namely the task of predicting which files are likely to be buggy in the future. In this work, we investigate whether these misclas- sifications also affect bug localization. To do so, we analyze issue reports that have been manually categorized by Herzig et al. and apply a bug localization technique to recover a ranked list of candidate buggy files for each issue report. We then evaluate whether the quality of ranked lists of reports reported as bugs is the same as that of real bug reports. Our findings shed light that there is a need for additional clean- ing steps to be performed on issue reports before they are used to evaluate bug localization techniques.
