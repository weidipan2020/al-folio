---
layout: page
title: notes
permalink: /notes/
description: Materials for courses you taught. Replace this text with your description.
nav: true
---

<div class="notes grid">
{% for note in site.notes | sort: 'title' %}
    <div class="items">
        <a href="{{ note.url | relative_url }}">{{ note.title }}</a>
    </div>
{% endfor %}
</div>