---
title: function-points
layout: repo
---

{% for post in site.categories.function-points do %}
    <div class="box">
        <h2>{{post.title}}</h2>
        <div class="block">
            {{post.content}}
        </div>
    </div>
{% endfor %}