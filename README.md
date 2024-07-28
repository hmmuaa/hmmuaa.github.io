个人内容
{% for file in site.static_files %}
* [{{ file.basename }}]({{ file.path | replace: '#','%23' }})
{% endfor %}

{% assign image_files = site.static_files | where: "image", false %}
{% for a in image_files %}
* [{{ a.basename }}]({{ a.path | replace: '#','%23' }})
{% endfor %}
