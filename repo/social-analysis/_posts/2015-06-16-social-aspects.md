---
title: JIRA
excerpt: "The JIRA Repository Dataset: Understanding Social Aspects of Software Development"
layout: repo-dataset
authors: "Bram Adams; Marco Ortu"
version: 4
---

#URL

* [Data Source (External)](https://www.dropbox.com/s/34n2t89exgsap8c/jira_backup_20141215.sql.zip?dl=0)
* [Paper in ACM Digital Library]()

#Change Log

When | What
---- | ----
June 15th, 2015 | Donated by [Marco Ortu](mailto:marco.ortu@diee.unica.it)

#Reference

Studies who have been using the data (in any form) are required to include the following reference:

```

```

#About the Data

##Overview of Data

Issue tracking systems store valuable data for testing hypotheses concerning maintenance, building statistical prediction models and recently investigating developers ``affectiveness". 
In particular, the Jira Issue Tracking System is a proprietary tracking system that has gained a tremendous popularity in the last years and offers unique features like the project management system and the Jira agile kanban board. 
This paper presents a dataset extracted from the Jira ITS of four popular open source ecosystems (as well as the tools and infrastructure used for extraction) the Apache Software Foundation, Spring, JBoss and CodeHaus communities. Our dataset hosts more than 1K projects, containing more than 700K issue reports and more than 2 million issue comments. Using this data, we have been able to deeply study the communication process among developers, and how this aspect affects the development process. Furthermore, comments posted by developers contain not only technical information, but also valuable information about sentiments and emotions. 
Since sentiment analysis and human aspects in software engineering are gaining more and more importance in the last years, with this repository we would like to encourage further studies in this direction.

## Top projects in the corpus


##Paper Abstract

We present the first method for automatically mining code idioms from a corpus of previously written, idiomatic software projects. We take the view that a code idiom is a syntactic fragment that recurs across projects and has a single semantic purpose. Idioms may have metavariables, such as the body of a for loop. Modern IDEs commonly provide facilities for manually defining idioms and inserting them on demand, but this does not help programmers to write idiomatic code in languages or using libraries with which they are unfamiliar. We present Haggis, a system for mining code idioms that builds on recent advanced techniques from statistical natural language processing, namely, nonparametric Bayesian probabilistic tree substitution grammars. We apply Haggis to several of the most popular open source projects from GitHub. We present a wide range of evidence that the resulting idioms are semantically meaningful, demonstrating that they do indeed recur across software projects and that they occur more frequently in illustrative code examples collected from a Q&A site. Manual examination of the most common idioms indicate that they describe important program concepts, including object creation, exception handling, and resource management
