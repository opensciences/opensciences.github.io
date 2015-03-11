---
title: openeffort
excerpt: Estimating Development Effort in Free/Open Source Software Projects by Mining Software Repositories: A Case Study of OpenStack
layout: repo
author: GregorioRobles
---


#URL

  * [Terapromise link](https://terapromise.csc.ncsu.edu:8443/svn/repo/effort/other-effort/openeffort)
  * [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2597107)


#Change Log

When | What
---- | ----
March 11, 2015 | Donated by [Gregorio Robles](/repo/people)


#Reference

Studies who have been using the data (in any form) are required to add the following reference to their report/paper:

    @inproceedings{Robles:2014:EDE:2597073.2597107,
    author = {Robles, Gregorio and Gonz\'{a}lez-Barahona, Jes\'{u}s M. and Cervig\'{o}n, Carlos and Capiluppi, Andrea and Izquierdo-Cort\'{a}zar, Daniel},
    title = {Estimating Development Effort in Free/Open Source Software Projects by Mining Software Repositories: A Case Study of OpenStack},
    booktitle = {Proceedings of the 11th Working Conference on Mining Software Repositories},
    series = {MSR 2014},
    year = {2014},
    isbn = {978-1-4503-2863-0},
    location = {Hyderabad, India},
    pages = {222--231},
    numpages = {10},
    url = {http://doi.acm.org/10.1145/2597073.2597107},
    doi = {10.1145/2597073.2597107},
    acmid = {2597107},
    publisher = {ACM},
    address = {New York, NY, USA},
    keywords = {Effort estimation, free software, mining software repositories, open source},
    }

#About the Data

## Data
There are two types of data associated with this paper: author activity from OpenStack contributors and survey data from the contributors. In addition, the raw data from which the author activity data was extracted can be found here:
http://gsyc.urjc.es/~grex/repro/2014-msr-effort/openstack_versioning_system_metadata.mysql.gz

### Author Activity Data
-Rows represent individual authors (1626 total)
-Columns represent months starting in Jan 2010 (these are 0-padded before and after project)
-The actual author IDs can be found by cross-referencing output_author_ids_nobots.csv:
    http://gsyc.urjc.es/~grex/repro/2014-msr-effort/output_authors_ids_nobots.csv
-Number of commits per month: 
    http://gsyc.urjc.es/~grex/repro/2014-msr-effort/output_commits_nobots.csv
-Number of active days per month:
    http://gsyc.urjc.es/~grex/repro/2014-msr-effort/output_activity_nobots.csv

### Survey Response Data
This represents voluntary responses to a survey in which 131 individuals responded.
Survey questions are as follows:
```
1) Selection: On average, how many hours in a week have you spent in the project in the 
last six months?
(>40h, 40h, 30h, 20h, 10h, <5h)

2) Selection: How much of the time you spent in the project is devoted to coding? 
(>95%, approx. 75%, approx. 50%, approx. 25%, <10%)

3) Selection: Do you make at least one commit to the repository the days you code? 
(yes, no)

4) Selection: What do you consider yourself in the project? 
(full-time, part-time, occasional contributor)

5) Free-text box: Did you always work on the project the same amount of hours, or did you have 
different phases of commitment? If you had different phases, could you tell us about the various 
phases? (the graph below may help you, as it is based in your recorded activity in the repository)
```
The survey data has 4 columns which reflect questions 1-4 and two additional columns labeled "info" and "survey" **of which I can't seem to find a description.**

The original (anonymized) survey response data is here:
http://gsyc.urjc.es/~grex/repro/2014-msr-effort/answers_openstack.all.public.csv

This survey data was cleaned with a few respondents being removed and some responses being edited. A description of the cleaning process as well as the cleaned response data is here:
http://gsyc.urjc.es/~grex/repro/2014-msr-effort/survey_cleaning.txt
http://gsyc.urjc.es/~grex/repro/2014-msr-effort/answers_openstack.public.csv