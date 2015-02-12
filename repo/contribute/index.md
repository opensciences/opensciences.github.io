---
title: How to contribute
layout: repopage
---

Before we get started, please remember to create all issues pertaining to the retrieval of SE data and papers within the ["Content retrieval hangout" GitHub milestone](https://github.com/opensciences/opensciences.github.io/milestones/Content%20retrieval%20hangout). In addition to putting issues in the milestone, remember to appropriately tag new issues.

## 1. *Browse* conferences

* Go find a recent SE conference with papers that might have data related to empirical SE experiments.
* [Create one GitHub issue](https://github.com/opensciences/opensciences.github.io/issues/new) for each conference, and add the "Conference" label to each
    * Add each issue to the "Content retrieval hangout" milestone
    * Leave a comment with a hyperlink to the conference

## 2. *Chunk* each conference

* Divide the conference into chunks based on its table of contents
* [Create one GitHub issue](https://github.com/opensciences/opensciences.github.io/issues/new) for each chunk, and add the "Chunk" label to each
    * Add each issue to the "Content retrieval hangout" milestone
    * Leave a comment with a hyperlink to the specific chunk from the conference
    * Assign the chunk to a worker so he or she can explore that chunk for useful papers

## 3. Find each paper that *maybe has data*

* For each chunk assigned to you, search through the papers, searching for those that may have downloadable data associated with them
* [Create one GitHub issue](https://github.com/opensciences/opensciences.github.io/issues/new) for each paper that may have data, and add the "Maybe Has Data" label to each
    * Add each issue to the "Content retrieval hangout" milestone
    * Leave a comment with a hyperlink to the specific paper from the conference

## 4. Filter for *target paper*s

* For each "Maybe Has Data" paper, check if there is actually data to download. In some cases, there will be many downloads available. Probably only one of them is important. Figure out which download is important. You might have to email the paper owner.
* If the paper has no downloadable data, remove the "Maybe Has Data" label, add the "No Data" label, and close the issue.
* If the paper DOES have downloadable data, remove the "Maybe Has Data" label, and add the "Target Paper" label
    * Leave a comment with
        * A hyperlink to the relevant data download
        * Email addresses of the paper owners
        * The body of an email to the owners that basically says "Thanks for making your data readily available. We're adding it to the TeraPromise database. Please let us know if you do not want us to mirror your data."
            * DO NOT send this email. Just write it.
        * Some context notes about this data. This will ideally be in Git-flavored markdown, but if you can't do that, plaintext is fine.
            * For an example of (long-ish) context notes, see http://openscience.us/repo/defect/ck/tut.html and http://openscience.us/repo/defect/tut.html
    * Flip a coin. If it's heads, assign this "Target Paper" issue to CarterPape. If it's tails, assign it to reesjones (Mitch Rees-Jones).

## 5. *Submit* the job

* Mr. Rees-Jones and Mr. Pape will then add the data to the big repo, add the context notes to our small repo, and email the owners with the url for both.
* Relabel the issue to "Submitted" and close the issue.
