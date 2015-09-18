---
title: Community QA
excerpt: "Finding high-quality content in social media"
layout: repo-dataset
authors: "Eugene Agichtein; Carlos Castillo; Debora Donato; Aristides Gionis; Gilad Mishne"
version: 4
---

#URL

* [Data Source (External)](http://webscope.sandbox.yahoo.com/catalog.php?datatype=l)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=1341531.1341557)

#Change Log

When | What
---- | ----
September 10th, 2015 | Donated by [Eugene Agichtein](mailto:eugene@mathcs.emory.edu)

#Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{Agichtein:2008:FHC:1341531.1341557,
author = {Agichtein, Eugene and Castillo, Carlos and Donato, Debora and Gionis, Aristides and Mishne, Gilad},
title = {Finding High-quality Content in Social Media},
booktitle = {Proceedings of the 2008 International Conference on Web Search and Data Mining},
series = {WSDM '08},
year = {2008},
isbn = {978-1-59593-927-2},
location = {Palo Alto, California, USA},
pages = {183--194},
numpages = {12},
url = {http://doi.acm.org/10.1145/1341531.1341557},
doi = {10.1145/1341531.1341557},
acmid = {1341557},
publisher = {ACM},
address = {New York, NY, USA},
keywords = {community question answering, media, user interactions},
}
```

#About the Data

##Overview of Data

User-generated data varies significantly in terms of quality. Due to the massive volume of data at disposal, filtering it based on quality and relevance becomes a matter of importance. This paper analyses methods for eliciting feedback from the community to extract high quality content. The focus is mainly on Yahoo! Answers, since there is a vast amount of content and social interactions available in it. The procedure employed successfully manages to filter high quality content with near human accuracy.

##Paper Abstract

The quality of user-generated content varies drastically from excellent to abuse and spam. As the availability of such content increases, the task of identifying high-quality content sites based on user contributions --social media sites -- becomes increasingly important. Social media in general exhibit a rich variety of information sources: in addition to the content itself, there is a wide array of non-content information available, such as links between items and explicit quality ratings from members of the community. In this paper we investigate methods for exploiting such community feedback to automatically identify high quality content. As a test case, we focus on Yahoo! Answers, a large community question/answering portal that is particularly rich in the amount and types of content and social interactions available in it. We introduce a general classification framework for combining the evidence from different sources of information, that can be tuned automatically for a given social media type and quality definition. In particular, for the community question/answering domain, we show that our system is able to separate high-quality items from the rest with an accuracy close to that of humans.
