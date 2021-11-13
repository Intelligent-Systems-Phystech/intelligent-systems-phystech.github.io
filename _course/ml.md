---
title: Machine Learning
name: Machine Learning
type: bachelor
avatar:
site: www.machinelearning.ru/wiki/index.php?title=Машинное_обучение_%28курс_лекций%2C_К.В.Воронцов%29
---

<h3 class="title">{{ page.name }}</h3>

{% if page.avatar %}
<img width="300" src="{{site.baseurl}}/images/course/{{page.avatar}}">
{% endif %}

### Contact

{% if page.site %}
[{{page.site}}](https://{{page.site}})<br>
{% endif %}
