#### Ukulele TABs
{% assign fs = site.static_files | where_exp:'a','a.path contains "/Ukulele TABs/"' %}
{% for a in fs %}
* [{{ a.basename }}]({{ a.path | replace: '#','%23' }})
{% endfor %}

#### Portraits
{% assign fs = site.static_files | where_exp:'a','a.path contains "/Portraits/"' %}
{% for a in fs %}
* [{{ a.basename }}]({{ a.path | replace: '#','%23' }})
{% endfor %}
