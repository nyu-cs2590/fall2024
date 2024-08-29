---
layout: page
title: Staff
description: A listing of all the course staff members.
---

# Staff

<!--
Staff information is stored in the `_staffers` directory and rendered according to the layout file, `_layouts/staffer.html`.
-->

## Instructors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Section leader' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Teaching Assistants

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}

{% assign graders = site.staffers | where: 'role', 'Grader' %}
{% assign num_graders = graders | size %}
{% if num_graders != 0 %}
{% for staffer in graders %}
{{ staffer }}
{% endfor %}
{% endif %}
