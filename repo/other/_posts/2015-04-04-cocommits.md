---
title: conmodels
excerpt: "Synchronous Development in OSS"
layout: repo
authors: "Qi Xuan; Vladimir Filkov"
version: 5
---


#URL

  * [Data in Terapromise](https://terapromise.csc.ncsu.edu:8443/!/#repo/view/head/other/cocommit)
  * [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2568238)

#Change Log

When | What
---- | ----
April 03, 2015| Donated by [Qi Xuan](/repo/people/data-donors/promise5.html)


#Reference

Studies who have been using the data (in any form) are required to add the following reference to their report/paper:

```
@inproceedings{Xuan:2014:BTS:2568225.2568238,
 author = {Xuan, Qi and Filkov, Vladimir},
 title = {Building It Together: Synchronous Development in OSS},
 booktitle = {Proceedings of the 36th International Conference on Software Engineering},
 series = {ICSE 2014},
 year = {2014},
 isbn = {978-1-4503-2756-5},
 location = {Hyderabad, India},
 pages = {222--233},
 numpages = {12},
 url = {http://doi.acm.org/10.1145/2568225.2568238},
 doi = {10.1145/2568225.2568238},
 acmid = {2568238},
 publisher = {ACM},
 address = {New York, NY, USA},
 keywords = {OSS, collaboration, communication, synchronization},
} 
```

# About the Data
The authors obtained data for 31 OSS projects from the Apache Software Foundation  on March 24th, 2012. For  each project, the commit activities of developers on dierent  files are gathered from the corresponding Git repository while the email communication  activities  are  gathered  from  the  online  developer mailing lists.  For  each commit activity,  The authors recorded the developer ID, file ID, file type, the exact submitting time in seconds, and the numbers of added and deleted LOC in each file.  For  each communication activity,  The authors recorded the sender ID, receiver ID, and the sending  time  in  seconds. Note that, developers may have multiple aliases, which were resolved  by  using  a  semi-automatic  approach.
