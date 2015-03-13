---
title: Promise 4
layout: repopage
category: repo
---

So far in Promise 4, we have added the following datasets:

{% for post in site.categories.[page.category] limit:page.limit do %}
    <a href="{{post.url}}">
    <div class="box">
        <h2>{{post.title}}</h2>
        <div class="block">
            {{post.excerpt}}
        </div>
    </div>
    </a>
{% endfor %}