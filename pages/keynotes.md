---

title: Keynotes
layout: event_noheader-2.0
permalink: /program/keynotes/

---
<section class="member-list">
{% for keynote in site.data.keynotespeakers %}
{%- if keynote.logo -%}
<div style="float:left;"><a href="{{keynote.url}}" class="keynote-logo" style="filter:none;"><img src="{{keynote.logo}}"/></a></div>
{% else %}
<div style="float:left;"><a href="{{keynote.url}}" class="keynote-logo" style="filter:none;">{{keynote.name}}</a></div>
{%- endif -%}
{% endfor %}
</section>
