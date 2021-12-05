---
title: titles.course
permalink: /course/
---

{% for type in site.global.course.types %}

<div class="pos_header">
  <h3>{% t site.global.course.types.{{ type }} %}</h3>
</div>
<hr>
<div class="content list people">
  {% for course in site.course %}
    {% if course.type contains type %}
      <div class="list-item-people">
        <p class="list-post-title">
          {% if course.avatar %}
            <a href="{{ site.baseurl }}{{ course.url }}"><img class="profile-thumbnail" src="/images/course/{{course.avatar}}"></a>
          {% else %}
            <a href="{{ site.baseurl }}{{ course.url }}"><img class="profile-thumbnail" src="/images/course/default.jpg"></a>
          {% endif %}
          <a class="name" href="{{ site.baseurl }}{{ course.url }}">{% t courses.name.{{ course.id | split: "/" | last }} %}</a>
        </p>
      </div>    
    {% endif %}
  {% endfor %}
</div>

{% endfor %}
