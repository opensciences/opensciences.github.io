---
title: datatrieve
excerpt: datatrieve
layout: repo-dataset
author: Guenther Ruhe
---


This is data from the transition of the DATATRIEVE product from version 6.0 to
	         version 6.1 (carried out at Digital Engineering Italy).

# URL

  * [Data Link (DOI)](https://doi.org/10.5281/zenodo.439578)

# Change Log

When | What
---- | ----
January 15, 2005 | Donated by [Guenther Ruhe](/repo/people/data-donors/promise3.html)


# Past usage

A hybrid approach to analyze empirical software engineering data
       and its application to predict module fault-proneness in maintenance;
       Source 	Journal of Systems and Software archive;
       Volume 53,  Issue 3.  (September 2000);
       Pages: 225 - 237;
       Year of Publication: 2000;
       ISSN:0164-1212;
       Authors:
       Sandro Morasca 	
       Gunther Ruhe

# Relevant information

The DATATRIEVE product was undergoing both adaptive (DATATRIEVE was being transferred  from platform OpenVMS/VAX to platform OpenVMS/Alpha) and corrective maintenance (failures reported from customers were being fixed) at the Gallarate (Italy) site of Digital Engineering.

The DATATRIEVE product was originally developed in the BLISS language. BLISS is an  expression language. It is block-structured, with exception handling facilities, coroutines, and a macro system. It was one of the first non-assembly languages for operating system implementation.. Some parts were later added or rewritten in the C language. Therefore, the  overall structure of DATATRIEVE is composed of C functions and BLISS subroutines.

The empirical study of this data set reports only the BLISS part, by far the bigger one.  In what follows, we will use the term "module" to refer to a BLISS module, i.e., a set of   declarations and subroutines usually belonging to one file. More than 100 BLISS modules   have been studied. It was important to the DATATRIEVE team to better understand how the  characteristics of the modules and transition process were correlated with the code quality.

The objective of the data analysis was to study whether it was possible to classify modules as non-faulty or faulty, based on a set of measures collected on the project.


# Data

Number of records: 130

Number of attributes: 9
   * 8 condition attributes
   * 1 decision attribute

Attribute Information:

   1 LOC6_0: number of lines of code of module m in version 6.0.
   1 LOC6_1: number of lines of code of module m in version 6.1.
   1 AddedLOC: number of lines of code that were added to module m in version 6.1, i.e., they were not present in module m in version 6.0.
   1 DeletedLOC: number of lines of code that were deleted from module m in version 6.0, i.e.,   they were no longer present in module m in version 6.1.
   1 Different Blocks: number of different blocks module m in between versions 6.0 and 6.1.
   1 Modification Rate: rate of modification of module m, i.e.,   (AddedLOC + DeletedLOC) / (LOC6.0 + AddedLOC).
   1 Module Knowledge: subjective variable that expresses the project team's knowledge on   module m (low or high)
   1 ReusedLOC: number of lines of code of module m in version 6.0 reused in module m in    version 6.1.
   1 Faulty6_1: its value is 0 for all those modules in which no faults were found;   its value is 1 for all other modules.

Missing attributes: none

Class Distribution:
   * 0:   119 = 91.54%
   * 1:   11  =  8.46%
