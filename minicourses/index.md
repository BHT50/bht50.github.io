---
title: Minicourses
---
<h1>Minicourses</h1>

{% for minicourse in site.minicourses %}
    {% if minicourse.eventcode contains 'jayme3' %}
    <h2><a href="{{ minicourse.url }}">{{ minicourse.title }}</a></h2>
    <h4>{{ minicourse.vagas }}</h4>
    <p><b>Lecturer:</b> {{ minicourse.lecturer }}</p>
    <p><b>Dates:</b> {{ minicourse.dates }}</p>
    <p><b>Schedule:</b> {{ minicourse.schedule }}</p>
    {% endif %}
{% endfor %}

