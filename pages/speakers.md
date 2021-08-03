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
<li><h3 class='training-header'>{{ speaker.Title }}</h3></li>
<li class="training-desc">{{ speaker.Description }}</li>
    <ul>
        <li style="font-size:smaller;"><hr><div class="training-container"><div class="training-image" style="background-image:url('{{speaker.Image}}');"></div><div class='trainer-container'><a href="/trainers/#{{tr.TrainerId}}">{{speaker.Name}}</a></div></div><div class='trainer-container-mobile'><a href="/trainers/#{{speaker.TrainerId}}">{{speaker.Name}}</a></div>{{speaker.Biography}}</li>        
    </ul>
</ul>
</section>
{% endfor %}
