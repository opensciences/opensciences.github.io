---
title: Identifier Splitters
excerpt: "A Dataset for Evaluating Identifier Splitters"
layout: repo-dataset
authors: "David Binkley; Dawn Lawrie; Lori Pollock; Emily Hill; K. Vijay-Shanker"
version: 4
---

# URL

* [Data in tera-PROMISE](https://terapromise.csc.ncsu.edu:8443/!/#repo/view/head/msr/splitters)
* [Paper in IEEE Digital Library](ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=6624055)

# Change Log

When | What
---- | ----
September 18th, 2015 | Donated by [David Binkley](mailto:binkley@cs.loyola.edu)

# Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@INPROCEEDINGS{6624055,
author={Binkley, D. and Lawrie, D. and Pollock, L. and Hill, E. and Vijay-Shanker, K.},
booktitle={Mining Software Repositories (MSR), 2013 10th IEEE Working Conference on},
title={A dataset for evaluating identifier splitters},
year={2013},
pages={401-404},
keywords={computational linguistics;program interpreters;software engineering;source coding;constituent words;human splitting judgements;identifier splitter evaluation dataset;identifier splitting techniques;natural language information;software engineering;software evolution techniques;source code;Data mining;Educational institutions;Gold;Java;Software;Speech recognition},
doi={10.1109/MSR.2013.6624055},
ISSN={2160-1852},
month={May},
}
```

# About the Data

## Overview of Data

The oracle, found in the file loyola-udelaware-identifier-splitting-oracle (ludiso) consists of 2663 identifiers. These identifiers were split by volunteers using a web interface. In all 8522 splitting judgements were collected for 2731 identifiers. The data set was curated based on the sum of confidence associated with a particular split. In order to provide a single correct split in the oracle, the split receiving the highest confidence sum was used as the correct split. Of the 2731 identifers, 68 do not appear in the oracle because of ties. (These identifiers can be found in the raw data.) Details on the construction of the oracle can be found in "An empirical study of identifier splitting technique".

## Attribute Information

Each line of the oracle represents one of the 2663 remaining oracle identifiers and includes the following.

the identifier's unique identification number,
the original identifier as extracted from the source,
the dominant language of the program that the id was extracted from,
the program from which it was extracted,
the identifier as shown to subjects where a '-' denotes a hard split,
the number of splittings (always 1 in the oracle, but not in the raw data),
the identifier as split by users,
the number of confidences (1 - 5) and then each confidence.

## Paper Abstract

Software engineering and evolution techniques have recently started to exploit the natural language information in source code. A key step in doing so is splitting identifiers into their constituent words. While simple in concept, identifier splitting raises several challenging issues, leading to a range of splitting techniques. Consequently, the research community would benefit from a dataset (i.e., a gold set) that facilitates comparative studies of identifier splitting techniques. A gold set of 2,663 split identifiers was constructed from 8,522 individual human splitting judgements and can be obtained from www.cs.loyola.edu/~binkley/ludiso. This set's construction and observations aimed at its effective use are described.
