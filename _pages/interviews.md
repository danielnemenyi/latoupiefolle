---
layout: default
title: Interviews
permalink: /interviews
---

<h1>{{ page.title }}</h1>

<p>
{% for note in site.notes %}
	{% if note.type == 'interview' %}
		<a href="{{ note.title | slugify }}">{{ note.title }}</a>
	{% endif %}
{% endfor %}
</p>
