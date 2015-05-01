---
title: huihuaprediction
excerpt: "Defect Prediction between Software Versions with Active Learning and Dimensionality Reduction"
layout: repo
authors: "Huihua Lu; Ekrem Kocaguneli; Bojan Cukic"
version: 4
---

#URL

* [Data in Terapromise](https://terapromise.csc.ncsu.edu:8443/!/#repo/view/head/defect/other-defect/huihuaprediction)
* [Paper in IEEE Digital Library](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=6982637)

#Change Log

When | What
---- | ----
April 3rd, 2015| Donated by [Huihua Lu](/repo/people/data-donors/promise4.html)

#Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@INPROCEEDINGS{6982637, 
  author={Huihua Lu and Kocaguneli, E. and Cukic, B.}, 
  booktitle={Software Reliability Engineering (ISSRE), 2014 IEEE 25th International Symposium on}, 
  title={Defect Prediction between Software Versions with Active Learning and Dimensionality Reduction}, 
  year={2014}, 
  month={Nov}, 
  pages={312-322}, 
  doi={10.1109/ISSRE.2014.35}, 
  ISSN={1071-9458},
}
```

#About the Data

##Overview of Data

Release packages/files % with defects metrics

+ 2.0 377 / 6729 50.4% / 14.5% 41 / 32
+ 2.1 434 / 7888 4 4.7% / 10.8% 41 / 32
+ 3.0 661 / 10593 47.4% /14.8% 41 / 32

Table I describes the defect content in three successive
releases of Eclipse, 2.0, 2.1, 3.0, at two levels of granularity:
files and packages. The data set has been aggregated from the
release archives and a bug repository. The release archives,
CVS and more recently GIT, provide entries related to the
commit history of a system. In Bugzilla, one can map each 
bug report to a release. For classification purposes, we divide packages/files into two classes - those with and without defects.
The complexity metrics for each package/file can be computed

from the archived builds of Eclipse. We utilized the same
complexity metrics used in [15].

##Attibute Information

```
<!DOCTYPE defects [
<!ELEMENT defects (plug-in)+>
<!ATTLIST defects project CDATA #REQUIRED>
<!ATTLIST defects release CDATA #REQUIRED>
<!ATTLIST defects dataversion CDATA #REQUIRED>
<!ELEMENT plug-in (compilationunit, counts, package)>
<!ATTLIST plug-in name CDATA #REQUIRED>
<!ELEMENT package (compilationunit, counts, package)>
<!ATTLIST package name CDATA #REQUIRED>
<!ELEMENT counts (count , count)>
<!ELEMENT count EMPTY>
<!ATTLIST count id CDATA #REQUIRED>
<!ATTLIST count value CDATA #REQUIRED>
<!ATTLIST count avg CDATA #IMPLIED>
<!ATTLIST count compilationunits CDATA #IMPLIED>
<!ATTLIST count max CDATA #IMPLIED>
<!ELEMENT compilationunit (counts , fix*)>
<!ATTLIST compilationunit dir CDATA #REQUIRED>
<!ATTLIST compilationunit base CDATA #REQUIRED>
<!ATTLIST compilationunit filename CDATA #REQUIRED>
<!ELEMENT fix (message)>
<!ATTLIST fix kind CDATA #REQUIRED>
<!ATTLIST fix bug_id CDATA #REQUIRED>
<!ATTLIST fix revision_id CDATA #REQUIRED>
<!ATTLIST fix author CDATA #REQUIRED>
<!ELEMENT message (#PCDATA)>
]>
```


##Paper abstract

Accurate detection of defects prior to product
release helps software engineers focus verification activities on
defect prone modules, thus improving the effectiveness of software
development. A common scenario is to use the defects from
prior releases to build the prediction model for the upcoming
release, typically through a supervised learning method. As
software development is a dynamic process, fault characteristics
in subsequent releases may vary. Therefore, supplementing the
defect information from prior releases with limited information
about the defects from the current release detected early, seems to
offer intuitive and practical benefits. We propose active learning
as a way to automate the development of models which improve
the performance of defect prediction between successive releases.
Our results show that the integration of active learning with
uncertainty sampling consistently outperforms the corresponding
supervised learning approach. We further improve the prediction
performance with feature compression techniques, where feature
selection or dimensionality reduction is applied to defect data
prior to active learning. We observe that dimensionality reduction
techniques, particularly multidimensional scaling with random
forest similarity, work better than feature selection due to
their ability to identify and combine essential information in
data set features. We present the improvements offered by this
methodology through the prediction of defective modules in the
three successive versions of Eclipse.
