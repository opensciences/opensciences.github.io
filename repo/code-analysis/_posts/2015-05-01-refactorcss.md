---
title: refactorcss
excerpt: "Discovering refactoring opportunities in cascading style sheets"
layout: repo
authors: "Davood Mazinanian; Nikolaos Tsantalis; Ali Mesbah"
version: 4
---

#URL

* [Data in Terapromise](https://terapromise.csc.ncsu.edu:8443/!/#repo/view/head/code-analysis/refactorcss)
* [Paper in ACM, IEEE, OR WHATEVER IT IS Digital Library](http://dl.acm.org/citation.cfm?id=2635879)

#Change Log

When | What
---- | ----
May 1st, 2015 | Donated by [Davood Mazinanian](/repo/people/data-donors/promise4.html)

#Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{Mazinanian:2014:DRO:2635868.2635879,
   author = {Mazinanian, Davood and Tsantalis, Nikolaos and Mesbah, Ali},
   title = {Discovering Refactoring Opportunities in Cascading Style Sheets},
   booktitle = {Proceedings of the 22Nd ACM SIGSOFT International Symposium on Foundations of Software Engineering},
   series = {FSE 2014},
   year = {2014},
   isbn = {978-1-4503-3056-5},
   location = {Hong Kong, China},
   pages = {496--506},
   numpages = {11},
   url = {http://doi.acm.org/10.1145/2635868.2635879},
   doi = {10.1145/2635868.2635879},
   acmid = {2635879},
   publisher = {ACM},
   address = {New York, NY, USA},
   keywords = {Cascading style sheets, duplication, refactoring},
} 
```

#About the Data

##Overview of Data

Contains CSS code and **FSE'14.csv** which indicates different measures for CSS datasets.

##Attribute Information

 * size
 * sloc
 * num_selectors
 * num_base_sel
 * num_grouped_sel
 * num_decs
 * Ionly
 * IIOnly
 * IIIOnly
 * I-II
 * I-III
 * II-III
 * I-II-IIII
 * number_of_duplicated_declarations
 * selectors_with_duplicated_declaration
 * longest_dup
 * max_sup_longest_dup
 * clone_sets
 * refactoring_opportunities
 * applied_refactorings_count
 * number_of_positive_refactorings
 * size_after
 * number_of_order_dependencies
 * Refactoring-Opportunities-excluding-subsumed
 * Positive-Refactoring-Opportunities-excluding-ubsumed

##Paper Abstract

Cascading Style Sheets (CSS) is a language used for describing the look and formatting of HTML documents. CSS has been widely adopted in web and mobile development practice, since it enables a clean separation of content from presentation. The language exhibits complex features, such as inheritance, cascading and specificity, which make CSS code hard to maintain. Therefore, it is important to find ways to improve the maintainability of CSS code. In this paper, we propose an automated approach to remove duplication in CSS code. More specifically, we have developed a technique that detects three types of CSS declaration duplication and recommends refactoring opportunities to eliminate those duplications. Our approach uses preconditions that ensure the application of a refactoring will preserve the original document styling. We evaluate our technique on 38 real-world web systems and 91 CSS files, in total. Our findings show that duplication in CSS code is widely prevalent. Additionally, there is a significant number of presentation-preserving refactoring opportunities that can reduce the size of the CSS files and increase the maintainability of the code.
