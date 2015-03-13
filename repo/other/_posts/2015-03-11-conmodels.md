---
title: conmodels
excerpt: "Developers’ Code Context Models for Change Tasks"
layout: repo
authors: "Thomas Fritz; David C. Shepherd; Katja Kevic; Will Snipes; Christoph Bräunlich"
version: 4
---


#URL

  * [External (Github) link](https://github.com/abb-iss/Study-Artifacts-for-Code-Context-Models)
  * [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2635868.2635905)

# Authors

* Thomas Fritz
* David C. Shepherd
* Katja Kevic
* Will Snipes
* Christoph Bräunlich

#Change Log

When | What
---- | ----
March 11, 2015 | Donated by [Thomas Fritz](/repo/people/data-donors/promise4.html)


#Reference

Studies who have been using the data (in any form) are required to add the following reference to their report/paper:

    @inproceedings{Fritz:2014:DCC:2635868.2635905,
    author = {Fritz, Thomas and Shepherd, David C. and Kevic, Katja and Snipes, Will and Br\"{a}unlich, Christoph},
    title = {Developers' Code Context Models for Change Tasks},
    booktitle = {Proceedings of the 22Nd ACM SIGSOFT International Symposium on Foundations of Software Engineering},
    series = {FSE 2014},
    year = {2014},
    isbn = {978-1-4503-3056-5},
    location = {Hong Kong, China},
    pages = {7--18},
    numpages = {12},
    url = {http://doi.acm.org/10.1145/2635868.2635905},
    doi = {10.1145/2635868.2635905},
    acmid = {2635905},
    publisher = {ACM},
    address = {New York, NY, USA},
    keywords = {Context models, change task, navigation, search, user study},
    }

#About the Data

Thomas Fritz, Christoph Bräunlich, and David Shepherd conducted a study of twelve developers performing one of three change tasks using the Eclipse IDE for Java Developers. Here we publish the data collected during this study.  Our data consists of twelve transcripts of developer actions transcribed by hand from the approximately two hours of video collected from each participant. It also includes the patches they submitted as solutions and a drawing/description of the program elements and relationships necessary to complete their task. Further details on the study setup can be found in our paper. 

[Tech Report: Supporting Search and Navigation through Code Context Models](http://www.merlin.uzh.ch/publication/show/7426)

--
### Download: 
To download our data, including transcripts, developer models, developer patches, and source code snapshots use Git to download this repository or [click on this link](https://github.com/abb-iss/Study-Artifacts-for-Code-Context-Models/archive/master.zip) for a .zip version.

--
### **Task:** [#116 New task in History->Tasks not visible](http://sourceforge.net/p/rachota/bugs/116/)
**Project:** [Rachota](http://sourceforge.net/projects/rachota/), **Version:** 2.4, **Subjects:** R1, R2, R3, R4

--
### **Task:** [Save Failed - Data Loss Occurs - ID: 3420227](http://sourceforge.net/tracker/?func=detail&aid=3420227&group_id=7118&atid=107118)
**Project:** [Freemind](http://sourceforge.net/projects/freemind/), **Version:** 0.9.0 RC 15, **Subjects:** F1, F2, F3, F4

--
### **Task:** [#30 list position lost after sleep](http://sourceforge.net/p/jpwsafe/bugs/30/)
**Project:** [JPasswordSafe](http://sourceforge.net/projects/jpwsafe/), **Version:** 2.4, **Subjects:** J1, J2, J3, J4

--
## Example Developer Packet (R3)

![Developer Model](/repo/other/img/conmodels/R3 - Developer Model.jpg)
A drawing or description of the program elements (e.g., methods, classes, fields) that the developer needed to understand in order to complete his/her task

![Transcript in Excel](/repo/other/img/conmodels/R3 - Transcript in Excel.png)
Transcript of developer's actions when working (partial transcript shown here, entire transcript available in repository)

    diff --git a/Rachota/src/org/cesilko/rachota/gui/HistoryView.java b/Rachota/src/org/cesilko/rachota/gui/HistoryView.java
    index 51a4d70..243c8ab 100644
    --- a/Rachota/src/org/cesilko/rachota/gui/HistoryView.java
    +++ b/Rachota/src/org/cesilko/rachota/gui/HistoryView.java
    @@ -36,6 +36,7 @@
     import java.util.Enumeration;
     import java.util.Iterator;
     import java.util.Vector;
    +
     import javax.swing.JMenuItem;
     import javax.swing.JOptionPane;
     import javax.swing.JPopupMenu;
    @@ -45,12 +46,20 @@
     import javax.swing.tree.DefaultMutableTreeNode;
     import javax.swing.tree.TreePath;
     import javax.swing.tree.TreeSelectionModel;
    +
     import org.cesilko.rachota.core.Day;
     import org.cesilko.rachota.core.Plan;
     import org.cesilko.rachota.core.Settings;
     import org.cesilko.rachota.core.Task;
     import org.cesilko.rachota.core.Translator;
    -import org.cesilko.rachota.core.filters.*;
    +import org.cesilko.rachota.core.filters.AbstractTaskFilter;
    +import org.cesilko.rachota.core.filters.DescriptionFilter;
    +import org.cesilko.rachota.core.filters.DurationFilter;
    +import org.cesilko.rachota.core.filters.IdleFilter;
    +import org.cesilko.rachota.core.filters.KeywordFilter;
    +import org.cesilko.rachota.core.filters.PriorityFilter;
    +import org.cesilko.rachota.core.filters.PrivateFilter;
    +import org.cesilko.rachota.core.filters.StateFilter;
     
     /** Panel providing history view on tasks from the past.
      * @author Jiri Kovalsky
    @@ -242,6 +251,7 @@
                         tbTasks.getColumnModel().getColumn(i).setHeaderValue(filteredTasksTableModel.getColumnName(i));
                 }
             });
    +        
         }
         
         /** Returns font that should be used for all widgets in this component
    @@ -1605,6 +1615,7 @@
             txtFilteredTime.setText(Tools.getTime(filteredTasksTableModel.getTotalTime()));
             historyChart.setDays(getDays());
             updateTotalTime();
    +        filterTasks();
         }
         
         public class MouseActionAdapter extends MouseAdapter implements ActionListener {

A patch containing developer's changes
