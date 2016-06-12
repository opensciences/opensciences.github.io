---
title: ossreview
excerpt: "Modern Code Reviews in Open-Source Projects: Which Problems Do They Fix?"
layout: repo-dataset
authors: "Moritz Beller; Alberto Bacchelli; Andy Zaidman; Elmar Juergens"
version: 4
---


# URL

  * [Data in Terapromise](https://terapromise.csc.ncsu.edu/repo/issues/ossreview)
  * [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2597082)

# Change Log

When | What
---- | ----
March 11, 2015 | Donated by [Moritz Beller](/repo/people/data-donors/promise4.html)


# Reference

Studies who have been using the data (in any form) are required to add the following reference to their report/paper:

    @inproceedings{Beller:2014:MCR:2597073.2597082,
      author = {Beller, Moritz and Bacchelli, Alberto and Zaidman, Andy and Juergens, Elmar},
      title = {Modern Code Reviews in Open-source Projects: Which Problems Do They Fix?},
      booktitle = {Proceedings of the 11th Working Conference on Mining Software Repositories},
      series = {MSR 2014},
      year = {2014},
      isbn = {978-1-4503-2863-0},
      location = {Hyderabad, India},
      pages = {202--211},
      numpages = {10},
      url = {http://doi.acm.org/10.1145/2597073.2597082},
      doi = {10.1145/2597073.2597082},
      acmid = {2597082},
      publisher = {ACM},
      address = {New York, NY, USA},
      keywords = {Code Review, Defects, Open Source Software},
    }

# About the Data

## Datasets
These datasets reflect changes made to two software projects: ConQAT and GROMACS. These come from manually analyzed cases in TMS (Task Management System), which are sub-smpled due the large number of tasks for each product. The datasets changes\_conqat\_rand and changes\_gromacs\_rand each consist of a stratified random sample of 120 tasks from their respective projects, while changes\_conqat\_100 reflects the 100 most recently changed tasks from ConQAT.

These datasets are .odb databases, which can be opened with either LibreOffice Base or OpenOffice Base. Base is not included in the basic Ubuntu install of LibreOffice, but can be installed with "apt-get install libreoffice-base"

Each dataset includes two tables:
-ISSUES lists issue numbers, authors, reviewers, the type of issue tracker, and whether the issue was valid.  
-REVIEWS lists issue numbers, sparse counts of the types of changes made according to the dichotomy below, and the number of self-motivated changes.

### Change Taxonomy
Here is a chart of the classification of change types, pulled from the original paper:
https://www.dropbox.com/s/rvp4mq9eo1rcyv9/fig3\_screenshot.png?dl=0
Each type of change represented by columns in the REVIEWS table has a prefix corresponding to it's classification in this taxonomy.
Examples:
-A comments change would be listed as "E\_D\_T\_COMMENTS" where "E\_D\_T" corresponds to "Evolvability, Documentation, Textual"
-A GUI change would be listed as "F\_LA\_GUI" where "F\_LA" corresponds to "Functional, Larger Defects"

For more details on change types, see http://figshare.com/articles/Code\_Review\_Defects/689805
