---
layout: page
title: "Tags"
permalink: tags
---
---

<div class="page">
{% assign tags = site.tags | sort %}
<ul>
{% for tag in tags %}
 <li><a href="/tag/{{ tag | first}}/">{{ tag[0] | replace:'-', ' ' }} ({{ tag | last | size }}){% unless forloop.last %}, {% endunless %}</a></li>
{% endfor %}
</ul>

</div>
