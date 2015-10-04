---
title: Radomized Algorithms
excerpt: "A Practical Guide for Using Statistical Tests to Assess Randomized Algorithms in Software Engineering"
layout: repo-dataset
authors: "Andrea Arcuri; Lionel Briand"
version: 4
---

#URL

* [Paper in IEEE Digital Library](Lhttp://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=6032439)

#Change Log

When | What
---- | ----
September 7th, 2015 | Donated by [Andrea Arcuri](mailto:arcuri@simula.no)

#Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@INPROCEEDINGS{6032439,
author={Arcuri, A. and Briand, L.},
booktitle={Software Engineering (ICSE), 2011 33rd International Conference on},
title={A practical guide for using statistical tests to assess randomized algorithms in software engineering},
year={2011},
pages={1-10},
keywords={software engineering;statistical analysis;practical guide;randomized algorithms;snapshot representation;software engineering;statistical tests;Algorithm design and analysis;Context;Search problems;Software algorithms;Software engineering;Statistical analysis;Testing;bonferroni adjustment;confidence interval;effect size;non-parametric test;parametric test;statistical difference;survey;systematic review},
doi={10.1145/1985793.1985795},
ISSN={0270-5257},
month={May},}
```

#About the Data

##Overview of Data

The review of the current practices involving the use of statistical
testing to analyze randomized algorithms in software engineering showed that randomness was not properly taken into account in the research literature. This paper provides a set of practical guidelines on the use of statistical testing that are tailored to randomized algorithms in software
engineering applications, with a particular focus on verification and validation (including testing), and the specific properties and constraints they entail. The proposed guidelines for the use of statistical tests in experiments
comparing randomized algorithms are as follows:
a) Run each randomized algorithm at least 1000 times on each problem instance. If not possible, explain the reasons.
b) For detecting statistical differences, use the non-parametric Mann-Whitney U-test for intervalscale results and the Fisher exact test for dichotomous results.
c) Report all the obtained p-values, whether they are smaller than α or not, and not just whether differences are significant.
d) When analyzing more than two randomized algorithms, use pairwise comparisons followed by pairwise statistical tests and effect size measures.
e) If space permits, provide full statistics for the collected data, as for example mean, median, variance, min/max values, skewness, median and absolute deviation. You can also use Boxplots for the same.
f) To help the meta-analyses of published results across studies, report means and standard deviations. For dichotomous experiments, always report the values a and b (so that other types of effect sizes can be computed.
g) Always report standardized effect size measures.

##Attribute Information

KEYWORDS
(ii1) Randomized Algorithms: A randomized algorithm is an algorithm that employs a degree of randomness as part of its logic. The algorithm typically produces different results on every run when applied to the same problem instance in the hope of achieving good performance in the "average case" based on the collected data from a large enough number of runs.
(ii2) Statistical Difference: A newly developed randomized algorithm needs to be tested against the more simpler existing algorithms with respect to certain criteria depending on the problem at
hand and other contextual assumptions so as decide on which one is more efficient.
(ii3) Parametric and Non-Parametric Test: A parametric statistical test is one that makes assumptions about the parameters (defining properties) of the population distribution(s) from which one's data are drawn, while a non-parametric test is one that makes no such assumptions.
(ii4) Systematic review: Systematic reviews are used to gather, in an unbiased and comprehensive way, published research on a specific subject and analyze it. Systematic reviews are a useful tool to assess general trends in published research, and they are becoming increasingly common in software engineering.

NOTES
(iii1) Motivational Statements: The review of the current practices involving the use of statistical testing to analyze randomized algorithms in software engineering showed that randomness was not properly taken into account in the research literature. This paper provides a set of practical
guidelines on the use of statistical testing that are tailored to randomized algorithms in software engineering applications, with a particular focus on verification and validation (including testing), and the specific properties and constraints they entail.
(iii2) Sampling Procedures: The authors limited the analyses of the results obtained with randomized algorithms to the year 2009 as their goal was just to get a representative, recent sample to draw their conclusions on. They focussed on research venues dealing with all aspects of software engineering such as IEEE TSE, IEEE ICSE and International Symposium
on Search Based Software Engineering.
(iii3) Baseline Results: Analysis of the results obtained with randomized algorithms in software engineering research (IEEE TSE, IEEE ICSE, International Symposium on SSBSE) showed that the statistical analyses were either missing, inadequate, or incomplete. Furthermore, the number of runs or the number of times the particular randomized algorithm was executed was not enough to come to a definite conclusion. Thus, there was a need to devise practical guidelines for the use of statistical testing in assessing randomized algorithms in software engineering applications.

##Paper Abstract

Randomized algorithms have been used to successfully addre
ss many different types of software engineering problems. This type of algorithms employ a degree of randomness as part of their logic. Randomized algorithms are useful for difficult problems where a precise solution cannot be derived in a deterministic way within reasonable time. However, randomized algorithms produce different results on every run when applied to the same problem instance. It is hence important to assess the effectiveness of randomized algorithms by collecting data from a large enough number of runs. The use of rigorous statistical tests is then essential to provide support to the conclusions derived by analyzing such data. In this paper, we provide a systematic review of the use of randomized algorithms in selected software engineering venues in 2009. Its goal is not to perform a complete survey but to get a representative snapshot of current practice in software engineering research. We show that randomized algorithms are used in a significant percentage of papers but that, in most cases, randomness is not properly accounted for. This casts doubts on the validity of most empirical results assessing randomized algorithms. There are numerous statistical tests, based on different assumptions, and it is not always clear when and how to use these tests. We hence provide practical guidelines to support empirical research on randomized algorithms in software engineering.
