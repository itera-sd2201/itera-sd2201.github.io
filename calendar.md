---
layout: page
title: Calendar
description: Listing of course modules and topics.
---

# Calendar
This calendar will be updated each time new lecture videos or assignments are released. Each week outline will be added the week before, any future topics or assignemnts are subject to change.

{% for module in site.modules %}
{{ module }}
{% endfor %}
