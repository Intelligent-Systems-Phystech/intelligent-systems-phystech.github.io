---
title: Andrey Grabovoy
name: Andrey Grabovoy
position: gs
avatar: grabovoy_av.jpg
twitter:
joined: 2017
mail: grabovoy.av@phystech.edu
site: andriygav.github.io
scholar: scholar.google.com/citations?user=y8Nbp58AAAAJ&hl=ru
---

<h3 class="title">{{ page.name }}</h3>

{% if page.avatar %}
<img width="300" src="{{site.baseurl}}/images/people/{{page.avatar}}">
{% endif %}

### Contact

{% if page.site %}
[{{page.site}}](https://{{page.site}})<br>
{% endif %}

{% if page.mail %}
<i class="fa fa-envelope-o"></i> <a href="mailto:{{page.mail}}">{{page.mail}}</a> <br>
{% endif %}

{% if page.scholar %}
<i class="fa fa-bar-chart"></i> [google scholar](https://{{page.scholar}}) <br>
{% endif %}

<hr>

### Research Interests

TODO

### Bio

TODO

<hr>
