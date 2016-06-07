---
title: kartikmining
excerpt: "Mining questions asked by web developers"
layout: repo-dataset
authors: "Kartik Bajaj; Karthik Pattabiraman; Ali Mesbah"
version: 4
---

#URL

* [Data in Terapromise](https://terapromise.csc.ncsu.edu/!/#repo/view/head/other/kartikmining)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2597083)

#Change Log

When | What
---- | ----
April 9th, 2015 | Donated by [Kartik Bajaj](/repo/people/data-donors/promise4.html)

#Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{bajaj2014mining,
  title={Mining questions asked by web developers},
  author={Bajaj, Kartik and Pattabiraman, Karthik and Mesbah, Ali},
  booktitle={Proceedings of the 11th Working Conference on Mining Software Repositories},
  pages={112--121},
  year={2014},
  organization={ACM}
}
```

#About the Data

##Overview of Data

This dataset is a data dump containing data from June 2008 to March 2013. Note that Stack Overflow originated only in June 2008. Therefore, this dump includes all the questions and answers on Stack Overflow until March 2013.

Stack Overflow provides data dumps of all user generated data, including questions asked with the list of answers, the accepted answer per question, up/down votes, favourite counts, post score, comments, and anonymized user reputation. Stack Overflow allows users to tag discussions and has a reputation-based mechanism to rank users based on their active participation and contributions.

##Attribute Information

Attribute info the datasets are in xml format including questions and answers for the following topics:

 * CSS
 * CSS-mobile
 * HTML5
 * HTML5-mobile
 * JavaScript
 * Javascript-mobile

##Paper Abstract

Modern web applications consist of a significant amount of clientside code, written in JavaScript, HTML, and CSS. In this paper, we present a study of common challenges and misconceptions among web developers, by mining related questions asked on Stack Overflow. We use unsupervised learning to categorize the mined questions and define a ranking algorithm to rank all the Stack Overflow questions based on their importance. We analyze the top 50 questions qualitatively. The results indicate that (1) the overall share of web development related discussions is increasing among developers, (2) browser related discussions are prevalent; however, this share is decreasing with time, (3) form validation and other DOM related discussions have been discussed consistently over time, (4) web related discussions are becoming more prevalent in mobile development, and (5) developers face implementation issues with new HTML5 features such as Canvas. We examine the implications of the results on the development, research, and standardization communities.
