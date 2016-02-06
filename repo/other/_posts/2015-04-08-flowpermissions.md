---
title: flowpermissions
excerpt: "Information Flows as a Permission Mechanism"
layout: repo-dataset
authors: "Feng Shen; Namita Vishnubhotla; Chirag Todarka; Mohit Arora; Babu Dhandapani; Eric John Lehner; Steven Y. Ko; Lukasz Ziarek"
version: 4
---

# URL

* [Data in Terapromise](https://terapromise.csc.ncsu.edu:8443/!/#repo/view/head/other/flowpermissions)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2643018)

# Change Log

When | What
---- | ----
April 8th, 2015 | Donated by [Feng Shen](/repo/people/data-donors/promise4.html)

# Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{Shen:2014:IFP:2642937.2643018,
   author = {Shen, Feng and Vishnubhotla, Namita and Todarka, Chirag and Arora, Mohit and Dhandapani, Babu and Lehner, Eric John and Ko, Steven Y. and Ziarek, Lukasz},
   title = {Information Flows As a Permission Mechanism},
   booktitle = {Proceedings of the 29th ACM/IEEE International Conference on Automated Software Engineering},
   series = {ASE '14},
   year = {2014},
   isbn = {978-1-4503-3013-8},
   location = {Vasteras, Sweden},
   pages = {515--526},
   numpages = {12},
   url = {http://doi.acm.org/10.1145/2642937.2643018},
   doi = {10.1145/2642937.2643018},
   acmid = {2643018},
   publisher = {ACM},
   address = {New York, NY, USA},
   keywords = {android, information flow, permissions},
}
```

# About the Data

## Overview of Data

* Distinct Flow Graphs and Data (Using Categories)
  * *Distinct Flows by Malicious Category Using Full Flow Names* This graph depicts the frequency of flows appearing within each Malicious cateogry defined by the MalGenome project, and includes the popular applications we processed under the "Normal" category for comparison purposes. The frequency is defined by the number of applications within a category that use a particular flow, divided by the total number of applications in that category, and is represented by the size of the marks in the scatter plot.
  * *Distinct Flow Categories by Malicious Category, Level 1* This graph, similar to the one described above, depicts the frequency of flow minus one level of distinction. For example, the flow sources android.location.Location:getLatitude and android.location.Location:getLongitude are now grouped under android.location.Location, as are their corresponding sinks.
  * *Distinct Flow Categories by Malicious Category, Level 2* This graph, similar to the first one described above, depicts the frequency of flow minus two levels of distinction. For example, the flow sources android.location.Location:getLatitude and android.location.Location:getLongitude are now grouped under android.location, as are their corresponding sinks.
  * *Distinct Flow Categories by Malicious Category, Level 3* This graph, similar to the first one described above, depicts the frequency of flow minus three levels of distinction. For example, the flow sources android.location.Location:getLatitude and android.location.Location:getLongitude are now grouped under android, as are their corresponding sinks.
* Distinct Flow Graphs and Data (General Malware Vs. Normal)
  * *Distinct Flows Using Full Flow Names* This graph depicts the frequency of flows appearing within each Malicious cateogry defined by the MalGenome project, and includes the popular applications we processed under the "Normal" category for comparison purposes. The frequency is defined by the number of applications within a category that use a particular flow, divided by the total number of applications in that category, and is represented by the size of the marks in the scatter plot.
  * *Distinct Flows Cateogories, Level 1* This graph, similar to the first graph, depicts the frequency of flow minus one level of distinction. For example, the flow sources android.location.Location:getLatitude and android.location.Location:getLongitude are now grouped under android.location.Location, as are their corresponding sinks.
  * *Distinct Flows Cateogories, Level 2* This graph, similar to the first graph, depicts the frequency of flow minus one level of distinction. For example, the flow sources android.location.Location:getLatitude and android.location.Location:getLongitude are now grouped under android.location, as are their corresponding sinks.
  * *Distinct Flows Cateogories, Level 3* This graph, similar to the first graph, depicts the frequency of flow minus one level of distinction. For example, the flow sources android.location.Location:getLatitude and android.location.Location:getLongitude are now grouped under android, as are their corresponding sinks.

## Attribute info
	1. Category
	2. Flow Source
	3. Flow Sink
	4. Distinct APK count
	5. Total Distinct APKs

## Paper abstract

This paper proposes Flow Permissions, an extension to the Android permission mechanism. Unlike the existing permission mechanism, our permission mechanism contains semantic information based on information flows. Flow Permissions allow users to examine and grant per-app information flows within an application (e.g., a permission for reading the phone number and sending it over the network) as well as cross-app information flows across multiple applications (e.g., a permission for reading the phone number and sending it to another application already installed on the user’s phone). Our goal with Flow Permissions is to provide visibility into the holistic behavior of the applications installed on a user’s phone. In order to support Flow Permissions on Android, we have developed a static analysis engine that detects flows within an Android application. We have also modified Android’s existing permission mechanism and installation procedure to support Flow Permissions. We evaluate our prototype with 2,992 popular applications and 1,047 malicious applications and show that our design is practical and effective in deriving Flow Permissions. We validate our cross-app flow generation and installation procedure on a Galaxy Nexus smartphone.
