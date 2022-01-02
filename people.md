---
title: titles.people
permalink: /people/
---
{% for role in site.global.people.roles %}


{% if role != 'template' %}

<div class="pos_header">
  <h3 id="{% t site.global.people.roles.{{ role }} %}">{% t site.global.people.roles.{{ role }} %}</h3>
</div>
<hr>
<div class="list people">
  {% for profile in site.people %}
    {% if profile.position contains role %}
      <div class="list-item-people">
        <p class="list-post-title">
          {% if profile.avatar %}
            <a href="{{ site.baseurl }}{{ profile.url }}"><img class="profile-thumbnail" src="/images/people/{{profile.avatar}}"></a>
          {% else %}
            <a href="{{ site.baseurl }}{{ profile.url }}"><img class="profile-thumbnail" src="/images/people/default.jpg"></a>
          {% endif %}
          <a class="name" href="{{ site.baseurl }}{{ profile.url }}">{% t peoples.name.{{ profile.id | split: "/" | last }} %}</a>
        </p>
      </div>    
    {% endif %}
  {% endfor %}
</div>
{% endif %}

{% endfor %}
