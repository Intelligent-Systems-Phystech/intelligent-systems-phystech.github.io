---
title: People
permalink: /people/
---
{% for role in site.global.people.roles %}


{% if role.id != 'template' %}

<div class="pos_header">
  <h3>{{ role.name }}</h3>
</div>

<div class="content list people">
  {% for profile in site.people %}
    {% if profile.position contains role.id %}
      <div class="list-item-people">
        <p class="list-post-title">
          {% if profile.avatar %}
            <a href="{{ site.baseurl }}{{ profile.url }}"><img class="profile-thumbnail" src="{{site.baseurl}}/images/people/{{profile.avatar}}"></a>
          {% else %}
            <a href="{{ site.baseurl }}{{ profile.url }}"><img class="profile-thumbnail" src="{{site.baseurl}}/images/people/default.jpg"></a>
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
