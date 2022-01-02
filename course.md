---
title: titles.course
permalink: /course/
---

{% for type in site.global.course.types %}

<div class="pos_header">
  <h3 id="{% t site.global.course.types.{{ type }} %}">{% t site.global.course.types.{{ type }} %}</h3>
</div>
<hr>
<div class="list course">
  {% for course in site.course %}
    {% if course.type contains type %}
      <div class="list-item-course">
        <p class="list-post-title">
          <a class="name" href="{{ site.baseurl }}{{ course.url }}">{% t courses.name.{{ course.id | split: "/" | last }} %}</a>
        </p>
      </div>    
    {% endif %}
  {% endfor %}
</div>

{% endfor %}
