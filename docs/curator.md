---
title: OpenScience Documentation
layout: repopage
---

# Curator
The Curator is responsible for adding datasets to tera-PROMISE as they are discovered. The datasets are discovered 
by data finders at "hackathons" (see the [contribute pages](/repo/contribute)) and each dataset is brought into the
workflow as a GitHub issue. The Curator then takes the GitHub issue and all of its corresponding information and
puts it in the repository, by taking context notes (a short description with metadata about the datasets, written
by data finders) and creating a description page ([example](/repo/other/dmtech.html)) on the GitHub site and then
uploading the data to an SVN repository.

# The general workflow of the Curator
 1. Find a GitHub issue for a paper/dataset to add
 2. Take the context notes from the issue and put it into a template description page ([example](/repo/other/dmtech.html))
 3. Put the newly created description page in the correct category within the GitHub site
 4. Download the data from the link found in the issue and upload it to the SVN repository
 5. Email the authors of the dataset/associated paper
 6. Close the GitHub issue

The Curator watches for [GitHub issues](https://github.com/opensciences/opensciences.github.io/issues)
(corresponding to papers/datasets) to pop up that have the appropriate labels which indicate that the issue has 
data and context notes and is ready for addition to the repo. The issue labels that the Curator deals with are 
as follows:

 * **4a. Target Paper**: Issue has data but no context notes.
 * **4b. Need to email authors**: Issue has relevant data, but there is no link so the authors must be emailed to locate the data.
 * **4e. Already have dataset**: That particular dataset has already been added to the repo, so doesn't need to be added again. 
 * **5. Summarized**: Issue has data AND context notes
 * **6. Submitted**: Issue has been completely added to the repo (with a description page, data uploaded to SVN, and authors emailed)
 * **7. Denied**: The authors of the dataset, after being notified via email that their data has been added to tera-PROMISE, email back asking to remove the dataset.

Data finders will label issues up to the point that they are **4x** or higher. The Curator then goes through each of the **5. Summarized** labels and creates a description page with the context notes provided in the issue (see below). If the data is missing (**4b. Need to email authors**), the Curator emails the authors asking for the data. If the dataset is already in the repo, **4e. Already have dataset** is added to the issue and closed.

Once the data has been added to the repo (description page and SVN) and the authors have been emailed (see below), **5. Summarized** is replaced with **6. Submitted** and the issue is closed. If the authors email back requesting the data to be removed (again, see below if confused), then **6. Submitted** is replaced with **7. Denied**. The issue should remain closed.

# Creating a description page
In opensciences.github.io/repo, there is a template.md file which contains all the necessary structure for a description page. The context notes from each GitHub issue should contain all information needed to fill in the template. The stuff in the context notes can be found [here](/repo/contribute/contextnotes.html), and transferring the context notes to the template is self-explanatory except for the "About The Data" section: the content of this will vary slightly across datasets, so best judgement should be used when filling in that section. Usually it'll just be the "General Overview of the Data" section from the context notes.

# Uploading data to the SVN repository



# Emailing dataset authors




