---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
---

## In Progress
---
{% bibliography --template bibtemplate --file In Progress --style _bibliography/cocolab_style.csl %}


<br />

## Published
---
{% for year in (2013..2017) reversed %}
### {{year}}

{% bibliography  --template bibtemplate --file Published --style _bibliography/cocolab_style.csl --query @*[year={{year}}] %}

{% endfor %}
