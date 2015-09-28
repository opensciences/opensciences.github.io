---
title: Software Aging and Rejuvenation
layout: repo-category
category: software-aging
---

Software Aging and Rejuvenation (SAR) research is about investigating defects in long-running software that cause the
gradual performance degradation and an increase of the failure rate with execution time.
Memory leaks are very simple example of software aging issue, but more types of software
aging exist. SAR research also looks for "rejuvenation" approaches to mitigate aging.
The nightly reboot of a system (when the load is very low, and thus the reboot is noticed by few users)
is an example of simple approach to prevent more severe software aging failures at unexpected times
(for example, users would like to avoid a sudden crash during load peaks, which would incur in high money losses).

SAR research investigates approaches to anticipate aging failures, for instance by using
time series analysis, and by using formal models (such as Petri nets and Markov chains) to schedule
the optimal rejuvenation time (the rejuvenation period should be high enough to avoid useless rejuvenations,
but should be low enough to anticipate aging failures). A comprehensive survey of this research
can be found in the following paper: 

[Domenico Cotroneo, Roberto Natella, Roberto Pietrantuono, and Stefano Russo. 2014. A survey of software aging and rejuvenation studies. J. Emerg. Technol. Comput. Syst. 10, 1, Article 8 (January 2014), 34 pages.](http://dl.acm.org/citation.cfm?id=2539117)

In the last decade, a community of active researchers has formed around these topics.
Several publications on SAR have been presented at the ISSRE and at the DSN conferences;
moreover, there is a workshop series, WoSAR, that periodically takes place as satellite event
of the ISSRE conference. Some journal special issues on Elsevier and ACM journals have also
been published. 

More information can be found on the website of the WoSAR workshops:

* [WoSAR 2015](https://sites.google.com/site/wosar2015/)
* [WoSAR 2014](https://sites.google.com/site/wosar2014/)
* [WoSAR 2013](https://sites.google.com/site/wosar2013/)
* [WoSAR 2012](https://sites.google.com/site/wosar2012/)

## Overview of Data

The data sets in this category are a collection of research artifacts in "Software Aging and Rejuvenation" (SAR). This is a growing repository with data being collected from SAR researchers and some of their well known studies. The artifacts that would be included in the repository are:

- Metrics on performance, resource consumption and failures collected at run-time from deployed software systems
- Metrics on performance, resource consumption and failures collected during stress tests of software systems
- Datasets on software aging bugs (similarly to datasets for defect prediction studies), by including software complexity metrics
- Models for rejuvenation scheduling (i.e., textual files for software reliability modeling tools, such as [SHARPE](http://sharpe.pratt.duke.edu/))

## Reference
Studies who have been using the data (in any form) are required to include the following reference:
``` 
@inproceedings{sarry,
  title={The Software Aging and Rejuvenation Repository},
  author={Cotroneo, Domenico and Iannillo, Antonio Ken and Natella, Roberto and Pietrantuono, Roberto and Russo, Stefano},
  booktitle={Software Aging and Rejuvenation (WoSAR), 2015 IEEE 7th Intl. Workshop on},
  year={2015},
  organization={IEEE}
}
```
## Data 

