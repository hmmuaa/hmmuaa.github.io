# Portraits
{% assign fs = site.static_files | where: "extname", '.jpg' %}
{% for a in fs %}
* [{{ a.basename }}]({{ a.path | replace: '#','%23' }})
{% endfor %}

##### test
{% for a in site.static_files | where: "extname", '.jpg' %}
* [{{ a.basename }}]({{ a.path | replace: '#','%23' }})
{% endfor %}
