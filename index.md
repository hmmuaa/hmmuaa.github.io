index
{% for file in site.static_files %}
* [{{ file.basename }}]({{ file.path | replace: '#','%23' }})
{% endfor %}


# Portraits
{% assign fs = site.static_files | where: "extname", '.jpg' %}
{% for a in fs %}
* [{{ a.basename }}]({{ a.path | replace: '#','%23' }})
{% endfor %}
