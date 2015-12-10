---
title: Tutorial on the CK Metrics
layout: repo-content
excerpt: Using OO Metrics
---

This page is about the Chidamber and Kemerer (CK) metrics.


## Overview

CK metrics are source code metrics that can be used for various purposes of analysis, e.g. defect prediction. The difference of CK metrics in comparison to McCabe and Halstead metrics is that CK metrics were designed specifically for source code developed in Object Oriented (OO) languages. The bibtex reference to CK metrics is given below:

```
       @Article{chidamber94,
                title   = "A metrics suite for object oriented design",
                author  = "Chidamber, S.R. and Kemerer, C.F.",
                pages   = "476--493",
                journal = "IEEE Transactions on Software Engineering",
                year    = "1994",
                volume  = "20",
                month   = "June",
                number  = "6"}
```

The CK metrics aim at measuring whether a piece of code follows OO principles. Hence, the proposed CK metrics are strongly related to OO concepts. The proposed CK metrics can be grouped under three stages of OO design processes:

+ Identification of Classes
+ Semantics of Classes
+ Relationship Between Classes

The definition of CK metrics as well as their distribution to the aforementioned OO design processes are as follows.


Identification of Classes:

+ Weighted Methods for Class (WMC): The sum of the complexities of each method in a class. If all the method complexities are considered equal and have the value of 1 (as proposed in the chidamber94), then WMC equals the number of methods in a class.
+ Depth of Inheritance Tree (DIT): Number of classes that a particular class inherits from.
+ Number of Children (NOC): The count of immediate subclasses of a class.

Semantics of Classes

+ Weighted Methods for Class (WMC): The sum of the complexities of each method in a class. If all the method complexities are considered equal and have the value of 1 (as proposed in the chidamber94), then WMC equals the number of methods in a class.
+ Response for Class (RFC): The number of elements in the response set of a class. The response set of a class (as defined in chidamber94) is the number of methods that can potentially be executed in response to a message received by an object of that class.
+ Lack of Cohesion of Methods (LCOM): For a class C, LCOM is the number of method pairs that have no common references to instance variables minus the number of method pairs that share references to instance variables.

Relationship Between Classes

+ Response for Class (RFC): The number of elements in the response set of a class. The response set of a class (as defined in chidamber94) is the number of methods that can potentially be executed in response to a message received by an object of that class.
+ Coupling Between Objects (CBO): For a class C, CBO is the number of classes that are coupled to (i.e. call a function or access a variable of) C.
+ A correspondence to the work of C&K was published by Churcher et al., where the authors discuss the practical implications of C&K metrics as well as ambiguities inherent in these metrics. The bibtex reference of the correspondence paper is given below:

```
       @Article{churcher95,
                title   = "Comments on 'A metrics suite for object oriented design' ",
                author  = "Churcher, N.I. and Shepperd, M.J. and Chidamber, S. and Kemerer, C.F.",
                pages   = "263--265",
                journal = "IEEE Transactions on Software Engineering",
                year    = "1995",
                volume  = "21",
                month   = "March",
                number  = "3"}
```

A brief and nice discussion concerning the pro's and con's of CK metrics can 
also be found [here](http://www.virtualmachinery.com/sidebar3.htm).

The CK metrics are also used in software defect prediction. For a short tutorial on defect prediction please refer here.

