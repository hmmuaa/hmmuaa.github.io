个人内容
{% for file in site.static_files %}
* [{{ file.basename }}]({{ file.path | replace: '#','%23' }})
{% endfor %}

# 2
{% assign fs = site.static_files %}
{% for a in fs %}
* [{{ a.basename }}]({{ a.path | replace: '#','%23' }})
{% endfor %}

# 3
{% assign fs = site.static_files | where: "extname", '.jpg' %}
{% for a in fs %}
* [{{ a.basename }}]({{ a.path | replace: '#','%23' }})
{% endfor %}
