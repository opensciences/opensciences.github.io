---
title: usecasedocs
excerpt: "Automatic early defects detection in use case documents"
layout: repo-dataset
authors: "Shuang Liu; Jun Sun; Yang Liu; Yue Zhang; Bimlesh Wadhwa; Jin Song Dong; Xinyu Wang"
version: 4
---

# URL

* [Data in Terapromise](https://terapromise.csc.ncsu.edu/repo/requirements/usecasedocs)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2642969)

# Change Log

When | What
---- | ----
April 8th, 2015 | Donated by [Shuang Liu](/repo/people/data-donors/promise4.html)

# Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{Liu:2014:AED:2642937.2642969,
   author = {Liu, Shuang and Sun, Jun and Liu, Yang and Zhang, Yue and Wadhwa, Bimlesh and Dong, Jin Song and Wang, Xinyu},
   title = {Automatic Early Defects Detection in Use Case Documents},
   booktitle = {Proceedings of the 29th ACM/IEEE International Conference on Automated Software Engineering},
   series = {ASE '14},
   year = {2014},
   isbn = {978-1-4503-3013-8},
   location = {Vasteras, Sweden},
   pages = {785--790},
   numpages = {6},
   url = {http://doi.acm.org/10.1145/2642937.2642969},
   doi = {10.1145/2642937.2642969},
   acmid = {2642969},
   publisher = {ACM},
   address = {New York, NY, USA},
   keywords = {natural language processing, use cases},
}
```

# About the Data

## Overview of Data

It has been reported that “More than 60% of the errors in a software product are committed during the design and less than 40% during coding."[1] and “Finding and fixing a software problem after delivery is often 100 times more expensive than finding and fixing it during the requirements and design phase" [2]. So finding defects in an early stage of software development is of great importance.

Use cases are widely used in Model-Driven Development to capture user requirements. Since the majority part of a use case document is written in natural language, it is thus highly desirable to rely on advanced natural language processing techniques to automatic the procedure of defects detection in use case documents.

###  Natural Language Parser

Zpar is a statistical muti-language parser. It has the state-of-the-art speed and accuracy for both Chinese and English on standard Penn Treebank data. Zpar provides word segmentation, part-of-speech tagging, dependency parsing and phrase structure parsing functionalities.

### Use Case Defect Finder (UCDF)

We developed a tool (UCDF) to automatically analysis use case documents and find defects. The source code is available here.

### Input Use Case Documents

We tested UCDF on two use case documents (for real systems). One is a stock trading system and the other is a personalized health informatics system for a reference implementation for IEEEP2407-compliant system. The stock trading system is in real use, thus the specifications of the system are confidential. We release the use case document for the personalized health informatics system, the automated guided vehicle system, the emergency monitoring system and the online shopping system.

## Paper Abstract

Use cases, as the primary techniques in the user requirement analysis, have been widely adopted in the requirement engineering practice. As developed early, use cases also serve as the basis for function requirement development, system design and testing. Errors in the use cases could potentially lead to problems in the system design or implementation. It is thus highly desirable to detect errors in use cases. Automatically analyzing use case documents is challenging primarily because they are written in natural languages. In this work, we aim to achieve automatic defect detection in use case documents by leveraging on advanced parsing techniques. In our approach, we first parse the use case document using dependency parsing techniques. The parsing results of each use case are further processed to form an activity diagram. Lastly, we perform defect detection on the activity diagrams. To evaluate our approach, we have conducted experiments on 200+ real-world as well as academic use cases. The results show the effectiveness of our method.
