---
layout: default
title: Digital Interfaces - Telecom Paris
---

# Digital Interfaces

{% for chapter in site.data.syllabus.chapters %}

{% if chapter.lectures %}
## {{ chapter.name }}

{% for lecture in chapter.lectures %}
- [{{ lecture.name }}]({{ site.baseurl }}/slides/{{ chapter.folder }}/{{ lecture.file }})
{% endfor %}
{% endif %}

{% endfor %}