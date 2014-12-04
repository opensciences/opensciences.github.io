---
title: bugreport
excerpt: bugreport recommender system data
layout: repo
author: Martin Pinzger, Emanuel Giger
---


#URL

  * With change log: https://terapromise.csc.ncsu.edu:8443/svn/repo/issues/bugreport.eclipse.jdt
  * With change log: https://terapromise.csc.ncsu.edu:8443/svn/repo/issues/bugreport.eclipse.platform
  * With change log: https://terapromise.csc.ncsu.edu:8443/svn/repo/issues/bugreport.gnome.evolution
  * With change log: https://terapromise.csc.ncsu.edu:8443/svn/repo/issues/bugreport.gnome.gstreamer
  * With change log: https://terapromise.csc.ncsu.edu:8443/svn/repo/issues/bugreport.mozilla.core
  * With change log: https://terapromise.csc.ncsu.edu:8443/svn/repo/issues/bugreport.mozilla.firefox


#Change Log

When | What
2010 | Donated by Martin Pinzger and Emanuel


#Reference

All data is licensed under the Creative Commons License 3.0. For more information on the license see http://creativecommons.org/licenses/by-sa/3.0/

Studies who have been using the data (in any form) are required to add the following reference to their report/paper:

&#123;&#123;&#123;
    @inproceedings&#123;Giger2010-rsse,
     author = &#123;Giger, Emanuel and Pinzger, Martin and Gall, Harald&#125;,
     title = &#123;Predicting the fix time of bugs&#125;,
     booktitle = &#123;Proceedings of the 2nd International Workshop on Recommendation Systems for Software Engineering&#125;,
     year = &#123;2010&#125;,
     location = &#123;Cape Town, South Africa&#125;,
     pages = &#123;52--56&#125;,
     publisher = &#123;ACM&#125;,
     address = &#123;New York, NY, USA&#125;,
    &#125; 
&#125;&#125;&#125;

#About the Data

== Short description of the data sources ==

The data files have been extracted from the eclipse, gnome, and mozilla bug repositories (many thanks goes to all the contributors of these projects). The data is until the year 2009.

Each row denotes the values extracted from one bug report. For each of the bug report attributes (listed below), we obtained the values at different points in time: current entry, the first entry (when the bug was reported), and the entries/measures after 1,3,7,14, and 30 days after the bug has been reported.

== List of bug report attributes ==

&#123;&#123;&#123;
    bugID
    component
    reporterEmail
    assigneeEmail
    os
    platform
    milestone
    nrKeywords
    nrDependentBugs
    peopleCC
    opened
    hoursOpenedBeforeNextRelease
    lastModified
    priority
    severity
    resolution
    firstFix
    lastFix
    hoursLastFixBeforeNextRelease
    hoursLastFixAfterPreviousRelease
    status
    firstActivity
    nrActivities
    lastResolution
    nrComments
    hoursToLastFix
    hoursToLastResolution
    monthOpened
    yearOpened
    monthYearOpened
    monthYearLastFixed
&#125;&#125;&#125;