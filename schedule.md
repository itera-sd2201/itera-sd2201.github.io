---
layout: page
title: 📆 Jadwal
description: The weekly event schedule.
---

# Jadwal Mingguan
{: #weekly-schedule }

{% for schedule in site.schedules %}
{{ schedule }}
{% endfor %}