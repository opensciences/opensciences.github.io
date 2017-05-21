---
title: Mandelbugs in Open-Source Software
excerpt: Software Aging and Rejuvenation
layout: repo-dataset
author: Roberto Natella
---

# URL

  - [Data Link (DOI)](http://wpage.unina.it/roberto.natella/datasets/mandelbugs_oss/)

### Author(s)

+ [Roberto Natella](mailto:roberto.natella@unina.it)

# Change Log

When | What
---- | ----
August 08th, 2015 | Donated by [Roberto Natella](mailto:roberto.natella@unina.it)

# Reference
Studies who have been using the data (in any form) are required to include the following reference:
```
@inproceedings{cotroneo2013fault,
  title={Fault Triggers in Open-Source Software: An Experience Report},
  author={Cotroneo, Domenico and Grottke, Michael and Natella, Roberto and Pietrantuono, Roberto and Trivedi, Kishor S},
  booktitle={Software Reliability Engineering (ISSRE), 2013 IEEE 24th International Symposium on},
  pages={178--187},
  year={2013},
  organization={IEEE}
}
```

# About the data

This dataset contains a list bugs from four open-source projects (the Linux kernel, the MySQL DBMS, the Apache HTTPD web server, and the Apache AXIS WS framework). The bugs have been classified into Mandelbugs, Bohrbugs, or Aging-Related Bugs, by analyzing the conditions that exercise the bug (i.e., the "fault trigger"). This classification is useful to get insights into bugs and failures that can occur in OSS projects, and to tune testing and fault-tolerance strategies according to the distribution of bug types in a project.

The dataset contains an ARFF file for each subsystem of the four open-source projects. Each row of the ARFF file contains:

- An IDs of the bug, which can be used to retrieve more information about the bug from the issue tracker of the project;

- A string that represents the class of the bug (BOH = Bohrbug; NAM = Mandelbug; ARB = Aging-Related Bug; UNK = Unknown class);

- A string that represents the sub-class of the bug (for Bohrbugs, the sub-class is not available; the subclasses for Mandelbugs are LAG, ENV, TIM, SEQ; the subclasses for Aging-Related bugs are MEM, STO, LOG, NUM, TOT).
