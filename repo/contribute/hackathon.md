---
title: How to fish for datasets
layout: repopage
---

We will be periodically hosting hackathons to track down and add SE data and papers.
{% if page.title %} {{site.hackathonInfo}}{% endif %}

# How to fish for software engineering data

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
    * If the paper has no downloadable data:
        * Remove the "Maybe Has Data" label, add the "No Data" label, and close the issue.
    * If the paper's data is data that is already in Terapromise:
        * Remove the "Maybe Has Data" label, add the "Already have dataset" label, and close the issue.
    * If the paper _does_ have downloadable data:
        * If, after downloading all relevant files and compressing it all together, the size of the compressed file is smaller than {{site.dataSizeCap}}:
            * Leave a comment with a hyperlink to the relevant data downloads. You'll need to spend some time figuring out the appropriate links.
            * Remove the "Maybe Has Data" label, and add the "Target Paper" label.
        * If the compressed file is larger than {{site.dataSizeCap}} but smaller than {{site.dataSizeAbsoluteCap}}:
            * Remove label "Maybe has data" and add label "Data maybe too big".
        * If the compressed file is larger than {{site.dataSizeAbsoluteCap}}:
            * Remove label "Maybe has data", add label "Data definitely too big", and close the issue.

## 5. *Summarize* the data
* 

## 6. *Submit* the job

* Carter Pape and Mitch Rees-Jones will then add the data to the big repo, add the context notes to our small repo, and email the owners with the url for both.
* Relabel the issue to "Submitted" and close the issue.
