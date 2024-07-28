# Portraits
{% assign fs = site.static_files | where: "extname", '.jpg' %}
{% for a in fs %}
* [{{ a.basename }}]({{ a.path | replace: '#','%23' }})
{% endfor %}

#### Ukulele TABs
{% assign fs = site.static_files | where_exp:'a','a.path contains "/Ukulele TABs/"' %}
{% for a in fs %}
* [{{ a.basename }}]({{ a.path | replace: '#','%23' }})
{% endfor %}
