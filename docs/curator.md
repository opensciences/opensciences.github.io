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

### Where to house the newly created description page
In the context notes, there should be a section called "Categorization", which lists the section that the dataset should be located within (for example: Defect, CK, Green Mining, etc. as seen on the sidebar). The github site, built on the Jekyll framework, houses the categories as folders in the website structure:

```
├── about
├── blog
│   └── _posts
├── contribute
│   └── _posts
├── defect
│   ├── ck
│   │   └── _posts
│   ├── mccabehalsted
│   │   └── _posts
│   └── other-defect
│       └── _posts
├── dump
│   └── _posts
├── effort
│   ├── cobol
│   │   └── _posts
...and so on
```
Within each category folder is a ```_posts``` folder, where Jekyll stores each description page. The newly created description page should be put in the ```_posts``` folder inside its corresponding category folder. For example, a description page of a dataset categorized as ```dump``` would be placed in ```/repo/dump/posts/[description page name].md```.

The naming convention for Jekyll posts (description pages) is:
```[year added, 4 digits]-[month added, 2 digits]-[day added, 2 digits]-[short name given to dataset].md```

The Curator chooses a succinct name for the dataset, no longer than 10ish characters. The name is often derived from the paper/dataset title, author name or initials, or some other unique identifier.

# Uploading data to the SVN repository
The Curator downloads the data from the link provided in the context notes (or emails the authors if the data is missing - the issue should have the label **4b. Need to email authors** if this is the case) and uploads it to the SVN repository as a zip file by adding a folder in the appropriate category and putting the data in it. If the data is excessively large, the data may need to be split up into multiple files as SVN doesn't handle large files particularly well.

Add the readme, change the link in the description page, and email authors.


# Emailing dataset authors

Openscience.content@gmail.com has a template email. Copy the contents and title, and replace the default information with the information about the dataset added. Email all authors listed in the context notes. The purpose of this email is to let the authors know that the data was added to the repository for their viewing pleasure and so they can offer suggestions on the context notes or request that we remove the data from the repository.



