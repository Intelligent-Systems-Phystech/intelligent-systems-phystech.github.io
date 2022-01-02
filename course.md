---
title: titles.course
permalink: /course/
---

{% for type in site.global.course.types %}

<div class="list-header">
  <h3 id="{% t site.global.course.types.{{ type }} %}">{% t site.global.course.types.{{ type }} %}</h3>
</div>
<hr>
<div class="list-course">
  {% for course in site.course %}
    {% if course.type contains type %}
    <a class="course-name" href="{{ site.baseurl }}{{ course.url }}">
      <div class="list-item-course">
        <p class="list-item-course-title">
          {% t courses.name.{{ course.id | split: "/" | last }} %}
        </p>
      </div>  
    </a>
    {% endif %}
  {% endfor %}
</div>

{% endfor %}
