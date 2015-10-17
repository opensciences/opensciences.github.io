---
title: Eclipse and Mozilla defect tracking dataset
excerpt: "The Eclipse and Mozilla defect tracking dataset: A genuine dataset for mining bug information"
layout: repo-dataset
authors: "Ahmed Lamkanfi, Javier Perez, Serge Demeyer"
version: 4
---

#URL

* [Data in tera-PROMISE](https://terapromise.csc.ncsu.edu:8443/!/#repo/view/head/defect/defect-other/defect-tracking)
* [Paper in Digital Library](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=6624028)

#Change Log

When | What
---- | ----
September 18th, 2015 | Donated by [Ahmed Lamkanfi](mailto:Ahmed.Lamkanfi@ua.ac.be)

#Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{lamkanfi2013eclipse,
  title={The eclipse and mozilla defect tracking dataset: a genuine dataset for mining bug information},
  author={Lamkanfi, Ahmed and P{\'e}rez, Javier and Demeyer, Serge},
  booktitle={Proceedings of the 10th Working Conference on Mining Software Repositories},
  pages={203--206},
  year={2013},
  organization={IEEE Press}
}
```

#About the Data

##Overview of Data

A dataset with over 200.000 reported bugs extracted from the Eclipse and Mozilla projects (respectively 47.000 and 168.000 reported bugs). Besides providing a single snapshot of a bug report, we also include all the incremental modifications as performed during the lifetime of the bug report.

[More Info](https://github.com/ansymo/msr2013-bug_dataset/blob/master/README.md#description)

##Paper Abstract

The analysis of bug reports is an important subfield within the mining software repositories community. It explores the rich data available in defect tracking systems to uncover interesting and actionable information about the bug triaging process. While bug data is readily accessible from systems like Bugzilla and JIRA, a common database schema and a curated dataset could significantly enhance future research because it allows for easier replication. Consequently, in this paper we propose the Eclipse and Mozilla Defect Tracking Dataset, a representative database of bug data, filtered to contain only genuine defects (i.e., no feature requests) and designed to cover the whole bug-triage life cycle (i.e., store all intermediate actions). We have used this dataset ourselves for predicting bug severity, for studying bug-fixing time and for identifying erroneously assigned components. Sharing these data with the rest of the community will allow for reproducibility, validation and comparison of the results obtained in bug-report analyses and experiments.
