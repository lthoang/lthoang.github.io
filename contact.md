---
layout: page
title: Contact
permalink: /contact/
---

{% for contact in site.contacts %}
<b class="capitalize">{{ contact[0] }}: </b>{{ contact[1] }}
{% endfor %}