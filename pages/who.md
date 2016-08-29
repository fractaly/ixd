---
layout: default
published: true
permalink: /who/
title: Who
order: 2
color: '#000'
---
We are the amazing people who studied interaction design, woho!
{% for category_hash in site.data.who %}
{% assign category = category_hash[1] %}
#### {{category.category}}
<ul style="list-style-type: square">
  {% for person in category.members %}
    <li>
      <span>
        {{person.name}}
        {% if person.email%}
          - <a href="mailto:{{person.email}}">email</a>
        {% endif %}
        {% if person.website%}
          - <a href="{{person.website}}" target="_blank"> website </a>
      {% endif %}
      </span>
    </li>
  {% endfor %}
</ul>
{% endfor %}
