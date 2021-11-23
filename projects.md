---
layout: page
title: Projects
permalink: /project/
---

{% assign items = site.projects | sort: 'date' | reverse %}
{% for item in items %}
<div>
  <div>
    {{ item.title }}
  </div>
  <div>
    <small>
        <small>
            {{ item.date | date: "%Y-%m-%d" }} | 
        </small>
        <small>
            {% if item.homepage %}<a href="{{ item.homepage }}">Homepage</a>{% endif %}
        </small>
    </small>
  </div>
  <div>
    <small>
        {{ item.description }}
    </small>
  </div>
</div>
<br>
{% endfor %}