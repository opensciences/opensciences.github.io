---
title: Data Categories
layout: repo-content
---

{% for category in site.datacategories %}
<div class="col-lg-3 col-md-4 col-sm-6 col-xs-6">
<div class="well">
<h3 class="page-header"><a href="{{category.repourl}}">{{category.title}}</a></h3>
{{category.description}}
</div>
</div>
{% endfor %}
