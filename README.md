个人内容

{% for file in site.static_files %}
* [{{ file.basename }}]({{ file.path|replace:'#,'%23' }})
{% endfor %}
