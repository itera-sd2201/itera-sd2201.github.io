---
layout: home
title: Home
nav_exclude: true
seo:
  type: Course
  name: SD2201 ITERA
---

# {{ site.tagline }}
{: .mb-2 }
{{ site.description }}
{: .fs-6 .fw-300 }

<!-- {% if site.announcements %}
{{ site.announcements.last }}
[Announcements](announcements.md){: .btn .btn-outline .fs-3 }
{% endif %} -->

## About the Class

Mata kuliah ini memberikan pemahaman dasar dan memodelkan permasalahan pemrograman menggunakan konsep pemrograman berbasis fungi untuk penyelesaian suatu permasalahan dengan implementasi menggunakan bahasa Python.

See the [Syllabus page](syllabus.md) for more details on course policies.

## Course Materials
{% for module in site.modules %}
{{ module }}
{% endfor %}

## Recent Announcements
{% assign num_recent_announcements = 2 %}
{% assign all_announcements = site.announcements | sort: "date" | reverse %}
{% for announcement in all_announcements limit:num_recent_announcements %}
  {{ announcement }}
{% endfor %}
[See All Announcements](#all-announcements){: .btn .btn-outline }

## Week 10 Schedule
{: #weekly-schedule }

{% for schedule in site.schedules %}
{{ schedule }}
{% endfor %}