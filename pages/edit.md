---
permalink: /edit
published: true
layout: default
title: 'edit'
hidden: true
order: 99999
---
<h3>Add</h3>
<h4>
  <a href="http://prose.io/#reimertz/ixd/new/master/_news" target="_blank">News</a>
  <a href="http://prose.io/#reimertz/ixd/tree/master/_news" target="_blank"><i>(see all)</i></a>
</h4>

<h4>
  <a href="http://prose.io/#reimertz/ixd/new/master/_projects" target="_blank">projects</a>
  <a href="http://prose.io/#reimertz/ixd/tree/master/_projects" target="_blank"><i>(see all)</i></a>
</h4>

<h4>
  <a href="http://prose.io/#reimertz/ixd/tree/master/_data/who" target="_blank">Who</a>
</h4>

<h3>Edit</h3>

{% assign sortedPages = site.pages | sort:"order" %}
{% for page in sortedPages %}
  {% if page.title !=  'index' and page.hidden != true %}
<h4><a href="http://prose.io/#reimertz/ixd/edit/master/{{ page.path }}" target="_blank">{{ page.path }}</a></h4>
  {% endif %}
{% endfor %}

