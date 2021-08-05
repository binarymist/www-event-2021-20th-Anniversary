---

title: Speakers
layout: event_noheader
permalink: /speakers/

---

# {{ page.title }}

{% assign talks = site.data.speakers | sort: 'Title' %}
{% for talk in talks %}
<section class="trainer-section">
<ul>
<li><a href="{{talk.TalkURL}}"><h3 class='training-header'>{{ talk.Title }}</h3></a></li>
<li class="training-desc"></li>
    <ul>
        {% for speaker in talk.Speakers %}
        <li style="font-size:smaller;"><div class="training-container"><div class="training-image" style="background-image:url('{{speaker.Image}}');"></div><div class='trainer-container'><a href="{{speaker.URL}}">{{speaker.Name}}</a></div></div><div class='trainer-container-mobile'><a href="{{speaker.URL}}">{{speaker.Name}}</a></div></li>
        {% endfor %}
    </ul>
</ul>
</section>
{% endfor %}