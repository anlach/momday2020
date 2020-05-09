---
layout: page
---
{% assign image_files = site.static_files | where: "image", true %}
{% for myimage in image_files %}
{{ myimage.path }}
<img src="{{ site.baseurl }}{{ myimage.path }}">
{% endfor %}