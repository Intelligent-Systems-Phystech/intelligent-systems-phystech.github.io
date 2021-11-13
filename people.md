---
title: People
permalink: /people/
---

{% assign peoples = site.people | sort: 'joined' %}

{% for role in site.global.people %}

<div class="pos_header">
{% role.name %}
</div>

{% if role.id != 'template' %}
<div class="content list people">
  {% for profile in peoples %}
    {% if profile.position contains role %}
      <div class="list-item-people">
        <p class="list-post-title">
          {% if profile.avatar %}
            <a href="{{ site.baseurl }}{{ profile.url }}"><img class="profile-thumbnail" src="{{site.baseurl}}/images/people/{{profile.avatar}}"></a>
          {% else %}
            <a href="{{ site.baseurl }}{{ profile.url }}"><img class="profile-thumbnail" src="http://evansheline.com/wp-content/uploads/2011/02/facebook-Storm-Trooper.jpg"></a>
          {% endif %}
          <a class="name" href="{{ site.baseurl }}{{ profile.url }}">{{ profile.name }}</a>
        </p>
      </div>    
    {% endif %}
  {% endfor %}
</div>
<hr>
{% endif %}
{% endfor %}
