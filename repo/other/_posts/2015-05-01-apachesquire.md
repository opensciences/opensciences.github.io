---
title: apachesquire
excerpt: "Project roles in the Apache Software Foundation: A dataset"
layout: repo-dataset
authors: "Megan Squire"
version: 4
---

# URL

* [Data Link (DOI)](https://doi.org/10.5281/zenodo.579735)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2487085.2487142)

# Change Log

When | What
---- | ----
May 1st, 2015 | Donated by [Megan Squire](/repo/people/data-donors/promise4.html)

# Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{Squire:2013:PRA:2487085.2487142,
   author = {Squire, Megan},
   title = {Project Roles in the Apache Software Foundation: A Dataset},
   booktitle = {Proceedings of the 10th Working Conference on Mining Software Repositories},
   series = {MSR '13},
   year = {2013},
   isbn = {978-1-4673-2936-1},
   location = {San Francisco, CA, USA},
   pages = {301--304},
   numpages = {4},
   url = {http://dl.acm.org/citation.cfm?id=2487085.2487142},
   acmid = {2487142},
   publisher = {IEEE Press},
   address = {Piscataway, NJ, USA},
}
```

# About the Data

## Overview of Data

Contains 3 tables in SQL format:

**Table 1 (apache_datasources):** List of Apache Data sources
Attributes (Name, Type):
  `datasource_id` Integer
  `item_description` Character
  `date_posted` Date
  `date_collected` Date
  `method` Character
  `item_url` Character
  `last_updated` Date

**Table 2(apache_people_projects):** List of people committing various projects
Attributes (Name, Type):
  `svn_id` Character
  `real_name` Character
  `web_site` Character
  `datasource_id` Integer
  `project_name` Character
  `role_on_project` Character
  `details` Character
  `email` Character
  `organization` Character
  `last_updated` Date

**Table 3(apache_unlisted_cla):** List of people with signed CLAs but are not committers
Attributes (Name, Type):
  `real_name` Character
  `datasource_id` Integer
  `last_updated` Date

## Paper Abstract


This paper outlines the steps in the creation and maintenance of a
new dataset listing leaders of the various projects of the Apache
Software Foundation (ASF). Included in this dataset are different
levels of committers to the various ASF project code bases, as well
as regular and emeritus members of the ASF, and directors and
officers of the ASF. The dataset has been donated to the FLOSSmole
project under an open source license, and is available for
[download](https://code.google.com/p/flossmole/downloads/detail?name=apachePeople2013-Jan.zip),
or for direct querying via a database client.
