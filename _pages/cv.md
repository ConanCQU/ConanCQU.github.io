---
layout: page
permalink: /cv/
title: CV
nav: true
nav_order: 3
description: Education, research experience, and honors.
toc:
  sidebar: left
---

{% assign cv = site.data.cv.cv %}

**{{ cv.name }}** · [Email](mailto:{{ cv.email }}) · [GitHub](https://github.com/ConanCQU)

## Education

{% for entry in cv.sections.Education %}

### {{ entry.institution }}

_{{ entry.studyType }} · {{ entry.area }}_

{% for item in entry.highlights %}

- {{ item }}
  {% endfor %}
  {% endfor %}

## Research experience

{% for entry in cv.sections.Projects %}

### {{ entry.name }}

{{ entry.summary }}

{% for item in entry.highlights %}

- {{ item }}
  {% endfor %}
  {% endfor %}

## Honors & awards

{% for entry in cv.sections['Honors and Awards'] %}

- **{{ entry.date }} · {{ entry.title }}** — {{ entry.summary }}
  {% endfor %}

## Languages

{% for entry in cv.sections.Languages %}
**{{ entry.name }}** · {{ entry.summary }}
{% endfor %}
