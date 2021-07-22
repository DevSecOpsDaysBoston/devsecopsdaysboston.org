---
layout: default
title:  "Agenda"
permalink: /agenda
---

<div class="flexbox">
  <a class="flexbox-button" href="{{ site.registration.relative_path }}">Attend {{ site.event_short_title }}</a>
  <a class="flexbox-button" href="/sponsor">Sponsor this Event</a>
</div>

# July 26th Live Stream Agenda
(Times are in Eastern / Atlantic EST time)

<style type="text/css">
tr td:first-of-type { white-space: nowrap; }
</style>

<div class="flexbox">

<div markdown="1" style="flex:1;align-self:flex-start;">

| Time | Session |
| 11:00 AM | Welcome and Intros |
| 11:15 AM | [Keynote: **Caroline Wong**<br />The Future of Cloud-Native Security](/speakers/caroline-wong)  |
| 12:00 PM | [Rob Cuddy: Raiders of the Lost AppSec](/speakers/rob-cuddy) |
| 12:25 PM | "Swarm Breakout" format intros |
| 12:30 PM | Sponsor swarm 1 - [CloudHealth Secure State](/sponsors/secure-state)   |
| 12:50 PM | [Prima Virani: How We Automated Ourselves Out of On-Call Burnout… and you can too!](/speakers/prima-virani) |
| 1:20 PM | [Vasant Chinnipilli: Rooting out security risks lurking in your kubernetes ecosystem](/speakers/vasant-chinnipilli) |
| 1:45 PM | [Nivedita Murthy: The Vulnerability Deluge: How to Dig In](/speakers/nivedita-murthy) |
| 2:10 PM | Breakout Sessions - Automating Security Checks |
| 2:30 PM | Stretch break; additional Sponsr shout-outs (3 slides) |
| 2:35 PM | [Mark Peters - Integrating DevSecOps Teams](/speakers/mark-peters) |
| 3:00 PM | [Ken Kato: DevOps in #CivicTech](/speakers/ken-kato) |
| 3:25 PM | [Panel Discussion - Growing and Sustaining Continuous Security Practices](/panel) |
| 4:00 PM | Wrap - All Organizers |

{% assign additionals = site.data.speakers.items | where_exp:"item", "item.additional" %}
{% if additionals.size > 0 %}

# Async Extras

<div class="flexbox" markdown=1>

  {% for person in additionals %}
    {% assign roledir = "speakers" %}
    {% if person.role == "panelist" %}{% assign roledir = "panelists" %}{% endif %}
| <a href="/{{ roledir }}/{{ person.id }}">{{ person.name }}<br />{{ person.title }}</a> |
  {% endfor %}
</div>
<div style="clear:both;width:100%;"></div>
{% endif %}


</div>

<div markdown="1" style="align-self:flex-start;">
  <img src="/assets/images/duck-dev.png" align="right" style="height:20em;margin-top:2em;" />
  <br />
  <img src="/assets/images/duck-ops.png" align="right" style="height:20em;margin-top:2em;" />
  <br />
  <img src="/assets/images/duck-sec.png" align="right" style="height:20em;margin-top:2em;" />
</div>

</div>

{% if site.data.speakers.items.size > 0 %}

# Speakers

{% include speaker-thumbs.html %}

{% endif %}
