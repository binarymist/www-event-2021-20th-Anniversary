---

title: Speakers
layout: event_noheader
permalink: /speakers/

---

# {{ page.title }}

{% assign speakers = site.data.speakers | sort: 'Name' %}
{% for speaker in speakers %}
<section class="trainer-section">
<hr>
<ul>
<li class="training-desc"><a href="{{speaker.TalkURL}}">{{ speaker.Title }}</a></li>
<li><div class="training-image" style="background-image:url('{{speaker.Image}}');"></div><h3 class='training-header'>{{ speaker.Name }}</h3></li>
</ul>
</section>
{% endfor %}
