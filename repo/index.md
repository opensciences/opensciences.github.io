---
title: Welcome to one of the largest repositories of SE research data
layout: repo-content
limit: 5
category: repo
---

The tera-PROMISE Repository is a **research dataset repository** specializing in software engineering research datasets. Sponsored by the [National Science Foundation](http://www.nsf.gov/), we provide **free** and **long-term** storage for **your research data**. Our goal is to 1. be a long-term storage facility for SE research data, and 2. to be a free and open platform for finding and hosting your datasets for the benefit of the research community as a whole. **Learn more** on our [about page](/repo/about).

You can view all of our datasets in the categories listed on the left and on the [categories page](/repo/categories).

<br>

<div class="row">
	<div class="col-lg-6 col-md-6">
		<div class="centered">
			<span class="glyphicon glyphicon-search glyphicon-h1-size" aria-hidden="true"></span>
			<h2><strong>Find research datasets</strong></h2>
			<p>We have everything from McCabe & Halsted to Spreadsheets to Green Mining.</p>
			<p><a class="btn btn-primary btn-lg" href="/repo/categories" role="button">View categories
			</a></p>
		</div>
	</div>
	<div class="col-lg-6 col-md-6">
		<div class="centered">
			<span class="glyphicon glyphicon-cloud-upload glyphicon-h1-size" aria-hidden="true"></span>
			<h2><strong>Contribute your data</strong></h2>
			<p>Learn how to contribute your research data, whether you're a researcher or a student.</p>
			<p><a class="btn btn-primary btn-lg" href="/repo/contribute" role="button">Learn how   
			</a></p>
		</div>
	</div>
</div>

<hr>

<div class="row">
	<div class="col-lg-6 col-md-6">
		<div class="well">
			<h2>Featured dataset</h2>
			
		</div>
	</div>
	<div class="col-lg-6 col-md-6">
		<div class="well">
			<h2>Latest News</h2>
			{% for newsitem in site.categories.news i| limit: 7 %}
				<p><strong>{{newsitem.date | date: '%B %d, %Y' }}:</strong> {{newsitem.title}}</p>
			{% endfor %}
		</div>
	</div>
</div>


## Most Recently Added Datasets (more [here](/repo/recent))
