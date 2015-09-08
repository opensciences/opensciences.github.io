---
title: Aging-related bugs and software complexity metrics
excerpt: Software Aging and Rejuvenation
layout: repo-dataset
author: Roberto Natella
---

# URL
 Data from authors website
 
  - [Aging related bugs metrics](http://wpage.unina.it/roberto.natella/datasets/aging_related_bugs_metrics/)
  
### Author(s)

+ [Roberto Natella](mailto:roberto.natella@unina.it)

# Change Log

When | What
---- | ----
August 08th, 2015 | Donated by [Roberto Natella](mailto:roberto.natella@unina.it)

# Reference
Studies who have been using the data (in any form) are required to include the following reference:
``` 
@article{cotroneo2013predicting,
  title={Predicting Aging-Related Bugs using Software Complexity Metrics},
  author={Cotroneo, Domenico and Natella, Roberto and Pietrantuono, Roberto},
  journal={Performance Evaluation},
  volume={70},
  number={3},
  pages={163--178},
  year={2013},
  publisher={Elsevier}
}
```
# About the data

This dataset contains information on aging-related bugs found in two open-source projects (the Linux kernel and the MySQL DBMS). This dataset has been used to investigate defect prediction approaches for aging-related bugs, by using software complexity metrics and machine learning techniques. New software complexity metrics were proposed in this study to support defect prediction ("aging-related" metrics).

The dataset contains an ARFF file for each subsystem of the open-source projects. Each row of the ARFF file contains:

- The name of a file in the project;

- "Program size" metrics for the file (columns from 2 to 50);

- "McCabe's cyclomatic complexity" metrics for the file (columns from 51 to 68);

- "Halstead" metrics for the file (columns from 69 to 77);

- "Aging-related" metrics for the file (columns from 78 to 83);

- The number of aging-related bugs found in the file.
