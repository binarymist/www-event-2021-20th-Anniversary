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
<ul style="min-height:100px;">
<li><div class="training-image" style="background-image:url('{{speaker.Image}}');"></div><a href="{{speaker.TalkURL}}"><h3 class='training-header'>{{ speaker.Title }}</h3></a></li>
<li class="training-desc"><a href="{{speaker.URL}}">{{ speaker.Name }}</a></li>
</ul>
</section>
{% endfor %}
