---
title: jzinference
excerpt: "Search-based inference of polynomial metamorphic relations"
layout: repo-dataset
authors: "Jie Zhang; Junjie Chen; Dan Hao; Yingfei Xiong; Bing Xie; Lu Zhang; Hong Mei"
version: 4
---

# URL

* [Data in Terapromise](https://terapromise.csc.ncsu.edu:8443/!/#repo/view/head/other/jzinference)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2642994)

# Change Log

When | What
---- | ----
 April 3rd, 2015 | Donated by [Jie Zhang](/repo/people/data-donors/promise4.html)

# Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{Zhang:2014:SIP:2642937.2642994,
  author = {Zhang, Jie and Chen, Junjie and Hao, Dan and Xiong, Yingfei and Xie, Bing and Zhang, Lu and Mei, Hong},
  title = {Search-based Inference of Polynomial Metamorphic Relations},
  booktitle = {Proceedings of the 29th ACM/IEEE International Conference on Automated Software Engineering},
  series = {ASE '14},
  year = {2014},
  isbn = {978-1-4503-3013-8},
  location = {Vasteras, Sweden},
  pages = {701--712},
  numpages = {12},
  url = {http://doi.acm.org/10.1145/2642937.2642994},
  doi = {10.1145/2642937.2642994},
  acmid = {2642994},
  publisher = {ACM},
  address = {New York, NY, USA},
  keywords = {invariant inference, metamorphic testing, particle swarm optimization},
}
```

# About the Data

## Overview of Data

directory
*this package contains all 1-MRs and 2-MRs our MRI inferred from the four libraries. Notice that all files are the original data our MRI produced, that is, all the MRs listed in this package are presented with a series of parameters.*
* MRs_apache
 1. MRs_apache[1-MRs inferred from Apache. Every function’s MRs are presented in the txt file in this directory named by the function’s name, including series of parameters, number of MRs, and the run time. Same to the other similar packages.]
 2. MRs_apache
* MRs_gsl
 1. MRs_gsl
 2. MRs_gsl
* MRs_jdk
 1. MRs_jdk
 2.MRs_jdk
* MRs_matlab
 1. MRs_matlab
 2. MRs_matlab
* time&MRnumber

*statistics on MR number and run time of all the MRs inferred from four libraries.*

## Paper abstract

Metamorphic testing (MT) is an effective methodology for testing those so-called “non-testable” programs (e.g., scientific programs), where it is sometimes very difficult for testers to know whether the outputs are correct. In metamorphic testing, metamorphic relations (MRs) (which specify how particular changes to the input of the program under test would change the output) play an essential role. However, testers may typically have to obtain MRs manually.

In this paper, we propose a search-based approach to automatic inference of polynomial MRs for a program under test. In particular, we use a set of parameters to represent a particular class of MRs, which we refer to as polynomial MRs, and turn the problem of inferring MRs into a problem of searching for suitable values of the parameters. We then dynamically analyze multiple executions of the program, and use particle swarm optimization to solve the search problem. To improve the quality of inferred MRs, we further use MR filtering to remove some inferred MRs.

We also conducted three empirical studies to evaluate our approach using four scientific libraries (including 189 scientific functions). From our empirical results, our approach is able to infer many high-quality MRs in acceptable time (i.e., from 9.87 seconds to 1231.16 seconds), which are effective in detecting faults with no false detection
