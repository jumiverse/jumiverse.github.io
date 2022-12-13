---
layout: page
---

<center>
  <h1>Archive</h1>
  {% for post in site.posts %}
    * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})
  {% endfor %}
</center>


