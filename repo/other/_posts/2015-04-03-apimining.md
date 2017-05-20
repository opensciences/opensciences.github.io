---
title: apimining
excerpt: "Statistical learning approach for mining API usage mappings for code migration"
layout: repo-dataset
authors: "Anh Tuan Nguyen; Hoan Anh Nguyen; Tung Thanh Nguyen; Tien N. Nguyen;"
version: 4
---

# URL

* [Data Link (DOI)](https://doi.org/10.5281/zenodo.439594)
* [Paper in ACM Digital Library](http://dl.acm.org/citation.cfm?id=2643010)

# Change Log

When | What
---- | ----
April 3rd, 2015| Donated by [Anh Tuan Nguyen](/repo/people/data-donors/promise4.html)

# Reference

Studies who have been using the data (in any form) are required to include the following reference:

```
@inproceedings{Nguyen:2014:SLA:2642937.2643010,
  author = {Nguyen, Anh Tuan and Nguyen, Hoan Anh and Nguyen, Tung Thanh and Nguyen, Tien N.},
  title = {Statistical Learning Approach for Mining API Usage Mappings for Code Migration},
  booktitle = {Proceedings of the 29th ACM/IEEE International Conference on Automated Software Engineering},
  series = {ASE '14},
  year = {2014},
  isbn = {978-1-4503-3013-8},
  location = {Vasteras, Sweden},
  pages = {457--468},
  numpages = {12},
  url = {http://doi.acm.org/10.1145/2642937.2643010},
  doi = {10.1145/2642937.2643010},
  acmid = {2643010},
  publisher = {ACM},
  address = {New York, NY, USA},
  keywords = {api mappings, api usages, code migration, statistical learning},
}
```

# About the Data

## Overview of Data

Manual migration of a large software project is a tedious, timeconsuming, and error-prone task. Toward reducing human effort in this task, there exist semi-automatic approaches and tools that help in language migration. Those tools/methods require users to define the migration rules/mappings between the corresponding Application Programming Interfaces (APIs) that are used in two languages. The existing tools/methods expect programmers to manually specify such API mappings. There is usually a large number of API mappings and many of them are newly introduced from time to time. Thus, existing tools can support only a subset of needed API mappings. As a result, the quality of the migrated code is reduced due to missing API mappings in such tools.

To reduce manual effort in defining the rules of API mappings for language migration, there exist approaches that automatically mine such API mappings from the corpus of the libraries’ client code that already has two corresponding versions in two languages. They all share the principle that two corresponding APIs and the usages in two languages have textually similar names, and the calling structures and parameters are similar. That principle and those heuristics might not always hold because in general, a library in the target language could use a quite different framework and different names of APIs than the library in the source language. A method call in a library might be replaced by a field access or by multiple statements in the target API. Even when it is replaced by a method call, the set of parameters might be different. Existing mining approaches also focus only on mapping of API methods/ classes, rather than entire API usages.

To address those challenges, we propose StaMiner, a data-driven model that statistically learns the mappings between entire API usages from the corpus of the corresponding methods in the client code of the APIs in two languages. Instead of using the heuristics as in the above deterministic methods, StaMiner is a statistical model that learns from the mappings in such a corpus. Currently, we focus on the API mappings between Java and C#. For each method, it builds a Groum, a graph representation for the API usages in the method. StaMiner extracts from the method’s Groum the connected sub-groums representing the API usages with one or multiple objects. For each of those sub-groums, it extracts its usage symbols. Then, the sequences of usage symbols for all sub-groums are put together separated by commas to form a sequence, called the sentence for the method. The sequences for sub-groums are placed in the sentence in the order of appearances of the first object in the code. The sentence for the respective method in C# is similarly built. Then, all the pairs of sentences for the corresponding methods are used as the input for a symbol-to-symbol alignment algorithm using Expectation-Maximization (EM). After that, StaMiner extends the resulting symbol-to-symbol alignments to compute the alignments for the sequences of symbols in two languages. The aligned sequences of symbols with their scores represent the mappings of API usages. Finally, the aligned sequences of symbols with scores higher than a threshold are presented in either the sequence or graph form.

The contributions of our work include:

 1. StaMiner: a novel, statistical learning method for mining API usage mappings between two languages.StaMiner also maps entire API usages;

 2. A tool to mine API usage mappings in Java and C#;
 3. An empirical evaluation to show StaMiner’s accuracy in mining API usages and supporting language migration.

## Paper abstract

The same software product nowadays could appear in multiple platforms and devices. To address business needs, software companies develop a software product in a programming language and then migrate it to another one. To support that process, semi-automatic migration tools have been proposed. However, they require users to manually define the mappings between the respective APIs of the libraries used in two languages. To reduce such manual effort, we introduce StaMiner, a novel data-driven approach that statistically learns the mappings between APIs from the corpus of the corresponding client code of the APIs in two languages Java and C#. Instead of using heuristics on the textual or structural similarity between APIs in two languages to map API methods and classes as in existing mining approaches, StaMiner is based on a statistical model that learns the mappings in such a corpus and provides mappings for APIs with all possible arities. Our empirical evaluation on several projects shows that StaMiner can detect API usage mappings with higher accuracy than a state-of-the-art approach. With the resulting API mappings mined by StaMiner, Java2CSharp, an existing migration tool, could achieve a higher level of accuracy.
