---
title: How to Donate Your Data
layout: repo-content
category: contribute
---


If you own or have access to data that you (and the author(s), if you are not an author) would like to be easily accessible through the Open Science repository, please fill out [this Google Form](http://goo.gl/7mWybm) with the appropriate information. You can also email the curators at [openscience.content@gmail.com](mailto:openscience.content@gmail.com). When we host data sets, we will include context notes about the data and the associated research. If possible, you should include in your email [context notes](/repo/contribute/#contextnotes) that we will use on the actual webpage for your data.


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
  <label class="col-md-4 control-label" for="category">Suggested category</label>  
  <div class="col-md-8">
  <input id="category" name="category" type="text" placeholder="Examples: Cocomo, Green Mining, NRP" class="form-control input-md" required="">
  </div>
</div>

<!-- Text input-->
<div class="form-group">
  <label class="col-md-4 control-label" for="link-to-dataset">Link to the dataset</label>  
  <div class="col-md-8">
  <input id="link-to-dataset" name="link-to-dataset" type="text" placeholder="Include all links if there are multiple" class="form-control input-md" required="">
    
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
  <input id="paper-link" name="paper-link" type="text" placeholder="Example: Paper in ACM Digital Library" class="form-control input-md">
    
  </div>
</div>

<!-- Textarea -->
<div class="form-group">
  <label class="col-md-4 control-label" for="authors">Attribution list for material</label>
  <div class="col-md-4">                     
    <textarea class="form-control" id="authors" name="authors">Example: an author list (include at least one email)</textarea>
  </div>
</div>

<!-- Textarea -->
<div class="form-group">
  <label class="col-md-4 control-label" for="bibtex">BibTeX Reference</label>
  <div class="col-md-4">                     
    <textarea class="form-control" id="bibtex" name="bibtex">This will be how others cite the data.</textarea>
  </div>
</div>

<!-- Textarea -->
<div class="form-group">
  <label class="col-md-4 control-label" for="overview">General overview of data</label>
  <div class="col-md-4">                     
    <textarea class="form-control" id="overview" name="overview">Provide us with some background info here.</textarea>
  </div>
</div>

<!-- Textarea -->
<div class="form-group">
  <label class="col-md-4 control-label" for="attributes">Attribute information</label>
  <div class="col-md-4">                     
    <textarea class="form-control" id="attributes" name="attributes">Give us some context about the attributes, if applicable.</textarea>
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
