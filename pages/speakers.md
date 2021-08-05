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
<li><div class="training-image" style="background-image:url('{{speaker.Image}}');"></div><h3 class='training-header'>{{ speaker.Name }}</h3></li>
<li class="training-desc">{{ speaker.Biography }}</li>
    <ul>
        <li style="font-size:smaller;"><hr><div class='trainer-container'><a href="{{speaker.URL}}"><strong>Title: {{speaker.Title}}</strong></a></div><div class='trainer-container-mobile'><a href="/trainers/#{{speaker.TrainerId}}">{{speaker.Title}}</a></div>{{speaker.Description}}</li>        
    </ul>
</ul>
</section>
{% endfor %}
