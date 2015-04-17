---
title: synthesis
excerpt: Search-Based Synthesis of Equivalent Method Sequences
layout: repo
author: Alberto Goffi
---

# URL
  * [Data in Terapromise](https://terapromise.csc.ncsu.edu:8443/svn/repo/defect/other/synthesis)
  * [Paper Link](http://software.imdea.org/~alessandra.gorla/papers/Goffi-SBES-FSE14.pdf)

### Author(s)
* Alberto Goffi
* Alessandra Gorla
* Andrea Mattavelli
* Mauro Pezzè
* Paolo Tonella

# Change Log

When | What
---- | ----
March 26th, 2015 | Donated by [Alberto Goffi](/repo/people/data-donors/promise4.html)

# About the Data

## Overview of Data

The authors ran their prototype on 47 methods of 7 classes taken from the Stack Java Standard Library and the Graphstream library. 123 equivalent method sequences were automatically synthesized, which represent more than 87% of the 141 sequences that were manually identified by the authors by inspecting the classes documentation. Those that could not be found due to the limitations of the prototype were excluded.

The authors have made available a replication package, containing both the subjects and
the data collected during their experiments. It is available at [http://star.inf.usi.ch/sb-synthesis](http://star.inf.usi.ch/sb-synthesis).

# Paper abstract

This paper proposes a search-based technique to synthesize
sequences of method invocations that are equivalent to a
target method within a finite set of execution scenarios.
The experimental results obtained on 47 methods from 7
classes show that the proposed approach correctly identifies
equivalent method sequences in the majority of the cases
where redundancy was known to exist, with very few false
positives.

