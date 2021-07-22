---
layout: default
title:  "Panel: Growing and Sustaining Security Practices"
permalink: /panel
---

<h1>{{ site.data.panel.title }}</h1>
<p>
  {{ site.data.panel.description }}
</p>
<div style="flex:1;align-self:flex-start;text-align:center;">
<div class="flexbox">
  <a class="flexbox-button" href="{{ site.registration_link }}" style="font-size:0.9em;">Attend this Session</a>
</div>
  <h3>Panelists</h3>
  <div class="flexbox" style="">
    {% assign panelists = site.data.speakers.items | where_exp:"item", "item.panel" %}
    {% for panelist in panelists %}
      {% include speaker-thumb.html person=panelist %}
    {% endfor %}
  </div>
</div>
