---
layout: page
title: Categories
permalink: /categories/
---

{% for cat in site.categories %}
{% assign nt = cat[0] %}

#### {{ nt }} {#cat-{{nt}}}
<ul> 
  {% for post in site.posts %}
     {% for pt in post.categories %}
    {% if nt == pt %}
      <li>
        {{post.published}} <a href="{{ post.url }}">{{ post.title }}</a>
      </li>
    {% endif %}  
   {% endfor %} 
  {% endfor %}
</ul>  
{% endfor %}


