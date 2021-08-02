---

title: Keynotes
layout: event_noheader-2.0
permalink: /https://github.com/OWASP/www-event-2021-20th-Anniversary/blob/master/_data/keynotes.yml/

---
<section class="member-list">
{% for keynote in site.data.keynote %}
{%- if keynote.logo -%}
<div style="float:left;"><a href="{{keynote.url}}" class="keynote-logo" style="filter:none;"><img src="{{keynote.logo}}"/></a></div>
{% else %}
<div style="float:left;"><a href="{{keynote.url}}" class="keynote-logo" style="filter:none;">{{keynote.name}}</a></div>
{%- endif -%}
{% endfor %}
</section>
