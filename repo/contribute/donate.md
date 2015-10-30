---
title: How to Donate Your Data
layout: repo-content
category: contribute
---


If you own or have access to data that you (and the author(s), if you are not an author) would like to be easily accessible through the Open Science repository, please fill out the following form with the appropriate information. You can also email the curators at [openscience.content@gmail.com](mailto:openscience.content@gmail.com).

When we host data sets, we will include context notes about the data and the associated research. If at all possible, you should include in your email [context notes](/repo/contribute/#contextnotes) that we will use on the actual webpage for your data.


<form class="form-horizontal" action="http://formspree.io/openscience.content@gmail.com" method="POST">
<fieldset>

<!-- Form Name -->
<legend>Donate your dataset (one per submission, please)</legend>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-4 control-label" for="suggest-name">Suggested name of dataset</label>
  <div class="col-md-8">
  <input id="suggest-name" name="suggest-name" type="text" placeholder="Preferably one word, under ~15 characters" class="form-control input-md">

  </div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-4 control-label" for="donator-info">Donator's Name and Email</label>
  <div class="col-md-8">
  <input id="donator-info" name="donator-info" type="text" placeholder="Name and Email" class="form-control input-md" required>

  </div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-4 control-label" for="category">Suggested category</label>
  <div class="col-md-8">
  <input id="category" name="category" type="text" placeholder="Examples: Cocomo, Green Mining, NRP" class="form-control input-md" required>
  </div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-4 control-label" for="link-to-dataset">Link to the dataset</label>
  <div class="col-md-8">
  <input id="link-to-dataset" name="link-to-dataset" type="url" placeholder="Include all links if there are multiple" class="form-control input-md" required>

  </div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-4 control-label" for="data-source">Data source *</label>
  <div class="col-md-8">
  <input id="data-source" name="data-source" type="text" placeholder="Example: a paper title, if applicable" class="form-control input-md" required="">

  </div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-4 control-label" for="paper-link">Link to the material associated with the dataset (if available)</label>
  <div class="col-md-8">
  <input id="paper-link" name="paper-link" type="url" placeholder="Example: Paper in ACM Digital Library" class="form-control input-md" required>

  </div>
</div>

<!-- Textarea -->
<div class="form-group">
  <label class="col-md-4 control-label" for="authors">Attribution list for material</label>
  <div class="col-md-4">
    <textarea class="form-control" placeholder="Example: an author list (include at least one email)" id="authors" name="authors"></textarea>
  </div>
</div>

<!-- Textarea -->
<div class="form-group">
  <label class="col-md-4 control-label" for="bibtex">BibTeX Reference</label>
  <div class="col-md-4">
    <textarea class="form-control" placeholder="This will be how others cite the data." id="bibtex" name="bibtex"></textarea>
  </div>
</div>

<!-- Textarea -->
<div class="form-group">
  <label class="col-md-4 control-label" for="overview">General overview of data</label>
  <div class="col-md-4">
    <textarea class="form-control" placeholder="Provide us with some background info here." id="overview" name="overview"></textarea>
  </div>
</div>

<!-- Textarea -->
<div class="form-group">
  <label class="col-md-4 control-label" for="attributes">Attribute information</label>
  <div class="col-md-4">
    <textarea class="form-control" placeholder="Give us some context about the attributes, if applicable." id="attributes" name="attributes"></textarea>
  </div>
</div>

<!-- Multiple Radios (inline) -->
<div class="form-group">
  <label class="col-md-4 control-label" for="part-of-a-larger-collection">Is this part of a larger series or collection?</label>
  <div class="col-md-4">
    <label class="radio-inline" for="part-of-a-larger-collection-0">
      <input type="radio" name="part-of-a-larger-collection" id="part-of-a-larger-collection-0" value="Yes" checked="checked">
      No
    </label>
    <label class="radio-inline" for="part-of-a-larger-collection-1">
      <input type="radio" name="part-of-a-larger-collection" id="part-of-a-larger-collection-1" value="No">
      Yes
    </label>
  </div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-4 control-label" for="link-to-larger-collection">If applicable, include a link to the larger collection</label>
  <div class="col-md-8">
  <input id="link-to-larger-collection" name="link-to-larger-collection" type="text" placeholder="" class="form-control input-md">

  </div>
</div>

<!-- Button -->
<div class="form-group">
  <label class="col-md-4 control-label" for="send-button"></label>
  <div class="col-md-4">
    <button id="send-button" name="send-button" class="btn btn-primary" type="submit">Send Message</button>
  </div>
</div>

<!-- Formspree hidden fields -->
<input type="hidden" name="_next" value="/repo/contribute/thanks.html" />
<input type="hidden" name="_subject" value="New submission from tera-PROMISE donation form" />
<input type="text" name="_gotcha" style="display:none" />


</fieldset>
</form>


## Help on the context notes

### 1. Data source
* Example: paper title, if this data is closely related to some original paper.

### 2. Link to the material associated with the dataset (if available)
* Examples:
    * A link to the ACM digital library (for example, [http://dl.acm.org/citation.cfm?id=2635868.2635905](http://dl.acm.org/citation.cfm?id=2635868.2635905))
    * A link to the IEEE digital library (for example, [http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=6982619](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=6982619))
    * Any other documentation

### 3. Attribution list for the material
* Include at least one contact email
* Example: author list for a paper

### 4. BibTeX reference
 * NOTE: This will be how others will cite the data.
 * Example: BibTeX for the paper

### 5. Link to the datasets
* If multiple files come with it, include links to all files, not just the parent file

### 6. PROMISE repo category (effort, requirements, model, defect, etc.)
* Categorize the data into one of the categories in the navbar on the [OpenScience website](/repo).
    * If it doesn't fit nicely into one of these categories, put "other" and propose a category name.

### 7. General overview of the data
* Note that, if the data is closely related to a paper, this will not be the abstract of the paper; it will be a general description of the data that provides context.

### 8. Attribute info
* If there are clearly defined columns or attributes to the data, describe each

### 9. Paper abstract (if appropriate)

### 10. Is this dataset part of a larger series or collection?
* If so, link to the master index of the series or collection (if possible)
