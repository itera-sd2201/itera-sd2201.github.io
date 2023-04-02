---
layout: home
title: Home
nav_exclude: true
---

# {{ site.tagline }}
{: .mb-2 }
{{ site.description }}
{: .fs-6 .fw-300 }

## Tentang Mata Kuliah

Mata kuliah ini memberikan pemahaman dasar dan memodelkan permasalahan pemrograman menggunakan konsep pemrograman berbasis fungsi untuk penyelesaian suatu permasalahan dengan implementasi menggunakan bahasa Python.

Lihat [silabus](syllabus.md) untuk lebih rinci.

## Pengumuman Terbaru
{% assign num_recent_announcements = 2 %}
{% assign all_announcements = site.announcements | sort: "date" | reverse %}
{% for announcement in all_announcements limit:num_recent_announcements %}
  {{ announcement }}
{% endfor %}
[Lihat semua pengumuman](announcements.md){: .btn .btn-outline }

## Jadwal Minggu Ini
{% for schedule in site.schedules %}
{{ schedule }}
{% endfor %}

## Modul Terbaru
{% assign num_recent_modules = 2 %}
{% assign all_modules = site.modules | sort: "date" | reverse %}
{% for module in all_modules limit:num_recent_modules %}
  {{ module }}
{% endfor %}
[Lihat semua modul](calendar.md){: .btn .btn-outline }
