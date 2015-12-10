---
title: Energy Mining
excerpt: "Mining energy-greedy API usage patterns in Android apps: an empirical study"
layout: repo-dataset
authors: "Mario Linares-Vásquez; Gabriele Bavota; Carlos Bernal-Cárdenas; Rocco Oliveto; Massimiliano Di Penta; Denys Poshyvanyk"
version: 4
---

#URL

* [Data in Terapromise](https://terapromise.csc.ncsu.edu:8443/!/#repo/view/head/code-analysis/apienergymining)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2597085)

#Change Log

When | What
---- | ----
April 9th, 2015 | Donated by [Mario Linares-Vásquez](/repo/people/data-donors/promise4.html)

#Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{Linares-Vasquez:2014:MEA:2597073.2597085,
  author = {Linares-V\'{a}squez, Mario and Bavota, Gabriele and Bernal-C\'{a}rdenas, Carlos and Oliveto, Rocco and Di Penta, Massimiliano and Poshyvanyk, Denys},
  title = {Mining Energy-greedy API Usage Patterns in Android Apps: An Empirical Study},
  booktitle = {Proceedings of the 11th Working Conference on Mining Software Repositories},
  series = {MSR 2014},
  year = {2014},
  isbn = {978-1-4503-2863-0},
  location = {Hyderabad, India},
  pages = {2--11},
  numpages = {10},
  url = {http://doi.acm.org/10.1145/2597073.2597085},
  doi = {10.1145/2597073.2597085},
  acmid = {2597085},
  publisher = {ACM},
  address = {New York, NY, USA},
  keywords = {Empirical Study, Energy consumption, Mobile applications},
} 
```

#About the Data

##Overview of Data

Excessive energy consumption in mobile apps can be a consequence of energy greedy hardware, bad programming practices, or particular API usage patterns. We present the largest to date quantitative and qualitative empirical investigation into the categories of API calls and usage patterns that—in the context of the Android development framework—exhibit particularly high energy consumption profiles. By using a hardware power monitor, we measure energy consumption of method calls when executing typical usage scenarios in 55 mobile apps from different domains. Based on the collected data, we mine and analyze energy-greedy APIs and usage patterns. We zoom in and discuss the cases where either the anomalous energy consumption is unavoidable or where it is due to suboptimal usage or choice of APIs. Finally, we synthesize our findings into actionable knowledge and recipes for developers on how to reduce energy consumption while using certain categories of Android APIs and patterns

## Abstract

Energy consumption of mobile applications is nowadays a hot topic, given the widespread use of mobile devices. The high demand for features and improved user experience, given the available powerful hardware, tend to increase the apps’ energy consumption. However, excessive energy consumption in mobile apps could also be a consequence of energy greedy hardware, bad programming practices, or particular API usage patterns. We present the largest to date quantitative and qualitative empirical investigation into the categories of API calls and usage patterns that—in the context of the Android development framework—exhibit particularly high energy consumption profiles. By using a hardware power monitor, we measure energy consumption of method calls when executing typical usage scenarios in 55 mobile apps from different domains. Based on the collected data, we mine and analyze energy-greedy APIs and usage patterns. We zoom in and discuss the cases where either the anomalous energy consumption is unavoidable or where it is due to suboptimal usage or choice of APIs. Finally, we synthesize our findings into actionable knowledge and recipes for developers on how to reduce energy consumption while using certain categories of Android APIs and patterns.