---
title: titles.course
permalink: /course/
meta_desc_en:  "Department of Intelligent Systems, academical courses at the Bachelor and Maste programme"
meta_desc_ru: "Кафедра интеллектуальных систем, курсы бакалавриата и магистратуры"
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
