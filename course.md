---
title: Course
permalink: /course/
---

{% for type in site.global.course.types %}

<div class="pos_header">
  <h3>{{ type.name }}</h3>
</div>
<hr>
<div class="content list people">
  {% for course in site.course %}
    {% if course.type contains type.id %}
      <div class="list-item-people">
        <p class="list-post-title">
          {% if course.avatar %}
            <a href="{{ site.baseurl }}{{ course.url }}"><img class="profile-thumbnail" src="{{site.baseurl}}/images/course/{{course.avatar}}"></a>
          {% else %}
            <a href="{{ site.baseurl }}{{ course.url }}"><img class="profile-thumbnail" src="{{site.baseurl}}/images/course/default.jpg"></a>
          {% endif %}
          <a class="name" href="{{ site.baseurl }}{{ course.url }}">{{ course.name }}</a>
        </p>
      </div>    
    {% endif %}
  {% endfor %}
</div>

{% endfor %}
