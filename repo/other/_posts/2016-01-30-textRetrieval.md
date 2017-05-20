---
title: Question Oriented Software Text Retrieval
excerpt: "Learning to Rank for Question-Oriented Software Text Retrieval"
layout: repo-dataset
authors: "Yanzhen Zou, Ting Ye, Yangyang Lu, John Mylopoulos, Lu Zhang"
version: 4
---

# URL

* [Data Link (DOI)](https://doi.org/10.5281/zenodo.581647)
* [Paper in IEEE Digital Library](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=7371990&filter%3DAND%28p_IS_Number%3A7371976%29)

# Change Log

When | What
---- | ----
January 29th, 2016 | Donated by [Yanzhen Zou](mailto:zouyz@pku.edu.cn)

# Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@INPROCEEDINGS{7371990,
author={Zou, Yanzhen and Ye, Ting and Lu, Yangyang and Mylopoulos, John and Zhang, Lu},
booktitle={Automated Software Engineering (ASE), 2015 30th IEEE/ACM International Conference on},
title={Learning to Rank for Question-Oriented Software Text Retrieval (T)},
year={2015},
pages={1-11},
keywords={Buildings;Feature extraction;Indexes;Search engines;Software;Software engineering;Training;classifier;interrogative;rank;text retrieval},
doi={10.1109/ASE.2015.24},
month={Nov},}
```

# About the Data

## Overview of Data

Dataset-1: Question-answer pairs on “Lucene” collected from StackOverflow. As mentioned in paper [36], we first get 5,587 questions and 7,872 answers from the StackOverflow with tag “lucene”, where 1,826 questions with positive votes are kept and labeled. We use these question and their 2,460 answers for original classifier training and testing.

Dataset-2: Question-answer pairs on “Java” collected from StackOverflow. We need more data to train the classifier models and evaluate our approach. Then we extend our data collection scope and randomly pick 50,000 questions with tag “Java” on StackOverflow. It may cost too much time if we judge the types of these question accurately and manually. We filter all the questions using regular expressions (e.g. the question includes phrases “how to” , “how can” or “what is the best way to”, etc., are labeled with “how to” tag). Finally, 11,003 questions and the corresponding 16,255 answers are selected. Table IV briefly describes these two datasets.

Dataset-3: FAQs of seven well-known open source projects. In software development, FAQs are used by many projects as part of their documentation. Compared with the data from StackOverflow, the FAQs are more formal and accurate. We want to investigate whether our approach is valid in search- ing these questions’ answers and whether the classifiers are affected by our learning examples. Table V illustrates the 7 open source projects and the numbers of their FAQs. All of them are the top level projects (TLPs) in Apache.

## Paper Abstract

Question-oriented text retrieval, aka natural language-based text retrieval, has been widely used in software engineering. Earlier work has concluded that questions with the same keywords but different interrogatives (such as how, what) should result in different answers. But what is the difference? How to identify the right answers to a question? In this paper, we propose to investigate the "answer style" of software questions with different interrogatives. Towards this end, we build classifiers in a software text repository and propose a re-ranking approach to refine search results. The classifiers are trained by over 16,000 answers from the StackOverflow forum. Each answer is labeled accurately by its question's explicit or implicit interrogatives. We have evaluated the performance of our classifiers and the refinement of our re-ranking approach in software text retrieval. Our approach results in 13.1% and 12.6% respectively improvement with respect to text retrieval criteria nDCG@1 and nDCG@10 compared to the baseline. We also apply our approach to FAQs of 7 open source projects and show 13.2% improvement with respect to nDCG@1. The results of our experiments suggest that our approach could find answers to FAQs more precisely.
