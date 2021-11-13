---
name: Name Surname
position: template
avatar: 
twitter:
joined: 
mail: 
site: 
scholar: scholar.google.com/citations?user=y8Nbp58AAAAJ&hl=ru
---

<img width="300" src="{{site.baseurl}}/images/people/{{page.avatar}}" data-action="zoom">

### Contact

{% if page.site %}
[{{page.site}}](https://{{page.site}})<br>
{% endif %}
<i class="fa fa-envelope-o"></i>  "{{page.mail}}" <br>
{% if page.scholar %}
<i class="fa fa-bar-chart"></i> [google scholar](https://{{page.scholar}}) <br>
{% endif %}

<hr>

### Research Interests

TODO

### Bio

TODO

<hr>
