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
 1. **Find a GitHub issue** with the label **5. Summarized**
 2. **Create a description page** by copying information from the GitHub issue into a template description page ([example](/repo/other/dmtech.html))
 3. **Move the new description page** in the correct category folder within the GitHub site
 4. **Download the data** from the link found in the issue and upload it to the SVN repository
 5. **Email the authors** of the dataset/associated paper
 6. **Close the GitHub issue**

# 1. Find a GitHub issue
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

# 2. **Create a description page**
In opensciences.github.io/repo, there is a template.md file which contains all the necessary structure for a description page. The context notes from each GitHub issue should contain all information needed to fill in the template. The stuff in the context notes can be found [here](/repo/contribute/contextnotes.html), and transferring the context notes to the template is self-explanatory except for the "About The Data" section: the content of this will vary slightly across datasets, so best judgement should be used when filling in that section. Usually it'll just be the "General Overview of the Data" section from the context notes.

### 3. **Move the description page** into the correct category folder
In the context notes, there should be a section called "Categorization", which lists the section that the dataset should be located within (for example: Defect, CK, Green Mining, etc. as seen on the sidebar). The GitHub site, built on the Jekyll framework, houses the categories as folders in the website structure:

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
Within each category folder is a ```_posts``` folder, where Jekyll stores the description pages. The newly created description page should be put in the ```_posts``` folder inside its corresponding category folder. For example, a description page of a dataset categorized as ```dump``` would be placed in ```/repo/dump/posts/[description page name].md```.

The naming convention for Jekyll posts (description pages) is:
```[year added, 4 digits]-[month added, 2 digits]-[day added, 2 digits]-[short name given to dataset].md```

The Curator chooses a succinct name for the dataset, no longer than 10ish characters. The name is often derived from the paper/dataset title, author name or initials, or some other unique identifier. Here's an example, if the description page called "example" was added on February 4th, 2015: 

```
2015-02-04-example.md
```

# 4. **Downloading and uploading data** to the SVN repository
The Curator downloads the data from the link provided in the context notes (or emails the authors if the data is missing - the issue should have the label **4b. Need to email authors** if this is the case) and uploads it to the SVN repository. The data should be contained in a zip file and named ```[dataset name].zip```. If the data is excessively large, the data may need to be split up into multiple zip files as SVN doesn't handle large files particularly well.

The SVN repository has a similar folder structure as the GitHub site, so the Curator adds a directory where the data will go. The new directory goes in the category that the dataset is in. For example, if adding the ```example``` dataset to the ```dump``` category, a directory called ```example``` is created in the ```dump``` folder, like so:

```
├── dump
│   └── example   <----
│   └── abacus2013
│   └── xorg
├── green-mining
│   └── greentrace
etc.
```

The zipped dataset is place in the ```example``` folder in this case, and then a ```README.txt``` is created.

The contents of the README will be:

```
To read/write comments on this data, see
 http://openscience.us/repo/PATH/TO/DESCRIPTION/PAGE.

```

This can usually be copied from another dataset as long as the link is changed.

# 5. **Email the dataset/paper authors**

After each dataset is added, the authors must be emailed. The purpose of this email is to let the authors know that the data was added to the repository for their viewing pleasure and so they can offer suggestions on the context notes or request that we remove the data from the repository. The email account **Openscience.content@gmail.com** is used to send the emails. In the drafts of the Gmail account, a template email has been constructed. Copy the contents and title of the email, and replace the default information with the information about the dataset added. DON'T delete the template email.

The email should be sent to ALL authors listed in the context notes. 

# 6. **Close the GitHub issue**

After the description page has been added, the data zipped and uploaded along with a README to the SVN repository in a new folder, and the email has been sent to the authors, the Curator relabels the GitHub issue for that particular dataset with **6. Submitted** and closes it.

----------------

# SVN/GitHub tips
 * To add a newly created directory or file to the SVN repository, navigate via command-line to the directory it's in and execute ```svn add [name of directory/file]```
 * To commit the changes, execute ```svn commit -m "Adds [dataset name] to repository"```
 * [Here](http://www.clear.rice.edu/comp314/svn.html) or [here](http://www.tutorialspoint.com/svn/) are good tutorials on SVN. Read up on it if you are confused.
 * To add newly created directories to the GitHub repository, use the same command as SVN except with ```git``` in front: ```git add [name of directory/file]```
 * Same with commit: ```git commit -m "Message"```
 * And [here](http://git-scm.com/doc) is arguably the best git tutorial (GitHub is the website that hosts projects that use ```git```, a version control system. If those last 3 words confused you, you should definitely read some of the tutorials. Start with the book if you're new to version control and start with the reference manual if you've already worked with it.
 
# Commit message tips

 * The commit messages for both GitHub and SVN should be of the form ```[verb]s [description]```. That's kind of vague, so here are some examples.
    * ```Updates README```
    * ```Adds example dataset description page```
    * ```Fixes dead link```
    * ```Adds new section to website```
    * ```Changes CSS```
    * etc.
 * Look through the commit history for more examples.
