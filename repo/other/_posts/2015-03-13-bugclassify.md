---
title: bugclassify
excerpt: "It’s Not a Bug, It’s a Feature: Does Misclassification Affect Bug Localization?"
layout: repo
author: PavneetSinghKochhar
---


#URL

* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2597105)
* [Data in Terapromise](https://terapromise.csc.ncsu.edu:8443/svn/repo/other/bugclassify)


#Change Log

When | What
---- | ----
March 13, 2015 | Donated by [Pavneet Singh Kochhar](/repo/people)


#Reference

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

#About the Data

To ensure representativeness, there are five popular, actively maintained software projects 
from three separate domains, namely desktop (Firefox and Eclipse), web (MediaWiki and Moodle), 
and mobile (Firefox Android). In addition, one commercial closed source application 
(Industrial) is included. The proprietary bug tracking system is from a Vancouver-based mobile 
app development company. The bug reports are filed by their testing team and end-users, and 
are related to different mobile platforms such as An- droid, Blackberry, iOS, and Windows 
Phone, as well as their content management platform and backend software.

##Abstract

Bug repository systems have become an integral component of software development activities. 
Ideally, each bug report should help developers to find and fix a software fault. However, 
there is a subset of reported bugs that is not (easily) re-producible, on which developers 
spend considerable amounts of time and effort. We present an empirical analysis of non-
reproducible bug reports to characterize their rate, nature, and root causes. We mine one 
industrial and five open-source bug repositories, resulting in 32K non-reproducible bug 
reports. We (1) compare properties of non-reproducible reports with their counterparts such as 
active time and number of authors, (2) investigate their life-cycle patterns, and (3) examine 
120 Fixed non-reproducible reports. In addition, we qualitatively classify a set of randomly 
selected non-reproducible bug reports (1,643) into six common categories. Our results show that, 
on average, non-reproducible bug reports pertain to 17% of all bug reports, remain active three 
months longer than their counterparts, can be mainly (45%) classified as “Interbug 
Dependencies”, and 66% of Fixed non-reproducible reports were indeed reproduced and fixed.


