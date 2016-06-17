---
title: bugreport
excerpt: bugreport recommender system data
layout: repo-dataset
author: MartinPinzger and EmanuelGiger
---


# URL

  * With change log:[https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.eclipse.jdt](https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.eclipse.jdt)
  * With change log:[https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.eclipse.platform](https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.eclipse.platform)
  * With change log:[https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.gnome.evolution](https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.gnome.evolution)
  * With change log:[https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.gnome.gstreamer](https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.gnome.gstreamer)
  * With change log:[https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.mozilla.core](https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.mozilla.core)
  * With change log:[https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.mozilla.firefox](https://terapromise.csc.ncsu.edu/repo/issues/bugreport/bugreport.mozilla.firefox)


# Change Log

When | What
---- | ----
January 1, 2010 | Donated by [Martin Pinzger](/repo/people/data-donors/promise3.html) and [Emanuel Giger](/repo/people/data-donors/promise3.html)


# Reference

All data is licensed under the Creative Commons License 3.0. For more information on the license see [http://creativecommons.org/licenses/by-sa/3.0/](http://creativecommons.org/licenses/by-sa/3.0/)

Studies who have been using the data (in any form) are required to add the following reference to their report/paper:

\{\{\{
    @inproceedings\{Giger2010-rsse,
     author = \{Giger, Emanuel and Pinzger, Martin and Gall, Harald\},
     title = \{Predicting the fix time of bugs\},
     booktitle = \{Proceedings of the 2nd International Workshop on Recommendation Systems for Software Engineering\},
     year = \{2010\},
     location = \{Cape Town, South Africa\},
     pages = \{52--56\},
     publisher = \{ACM\},
     address = \{New York, NY, USA\},
    \}
\}\}\}

# About the Data

## Short description of the data sources

The data files have been extracted from the eclipse, gnome, and mozilla bug repositories (many thanks goes to all the contributors of these projects). The data is until the year 2009.

Each row denotes the values extracted from one bug report. For each of the bug report attributes (listed below), we obtained the values at different points in time: current entry, the first entry (when the bug was reported), and the entries/measures after 1,3,7,14, and 30 days after the bug has been reported.

## List of bug report attributes

\{\{\{

   * bugID
   * component
   * reporterEmail
   * assigneeEmail
   * os
   * platform
   * milestone
   * nrKeywords
   * nrDependentBugs
   * peopleCC
   * opened
   * hoursOpenedBeforeNextRelease
   * lastModified
   * priority
   * severity
   * resolution
   * firstFix
   * lastFix
   * hoursLastFixBeforeNextRelease
   * hoursLastFixAfterPreviousRelease
   * status
   * firstActivity
   * nrActivities
   * lastResolution
   * nrComments
   * hoursToLastFix
   * hoursToLastResolution
   * monthOpened
   * yearOpened
   * monthYearOpened
   * monthYearLastFixed

\}\}\}
