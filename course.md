---
title: Course
permalink: /course/
---

{% assign course_sorted = site.course | sort: 'name' %}

{% if course_sorted.size == 0 %}
  {% continue %}
{% endif %}

<div class="content list people">
  {% for course in course_sorted %}
    <div class="list-item-people">
      <p class="list-post-title">
        {% if course.avatar %}
          <a href="{{ site.baseurl }}{{ course.url }}"><img class="profile-thumbnail" src="{{site.baseurl}}/images/course/{{course.avatar}}"></a>
        {% else %}
          <a href="{{ site.baseurl }}{{ course.url }}"><img class="profile-thumbnail" src="http://evansheline.com/wp-content/uploads/2011/02/facebook-Storm-Trooper.jpg"></a>
        {% endif %}
        <a class="name" href="{{ site.baseurl }}{{ course.url }}">{{ course.name }}</a>
      </p>
    </div>    
  {% endfor %}
</div>
<hr>