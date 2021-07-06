---
layout: default
title:  "Agenda"
permalink: /agenda
---

<div class="flexbox">
  <a class="flexbox-button" href="{{ site.registration.relative_path }}">Attend {{ site.event_short_title }}</a>
  <a class="flexbox-button" href="/sponsor">Sponsor this Event</a>
</div>

(Times are in Eastern / Atlantic EST time)

<style type="text/css">
tr td:first-of-type { white-space: nowrap; }
</style>

<div class="flexbox">

<div markdown="1" style="flex:1;align-self:flex-start;">

| Time | Session |
| 11:00 AM | Welcome and Intros |
| 11:15 AM | Keynote: **Caroline Wong**<br />The Future of Cloud-Native Security  |
| 12:00 PM | Rob Cuddy: Raiders of the Lost AppSec |
| 12:25 PM | "Swarm Breakout" format intros |
| 12:30 PM | Sponsor swarm 1   |
| 12:50 PM | Prima Virani: How We Automated Ourselves Out of On-Call Burnout… and you can too! |
| 1:15 PM | Vasant Chinnipilli: Rooting out security risks lurking in your kubernetes ecosystem |
| 1:40 PM | Stretch break; discussions check-in (screen share) |
| 1:45 PM | Nivedita Murthy: The Vulnerability Deluge: How to Dig In |
| 2:10 PM | Sponsor swarm 2 |
| 2:30 PM | Stretch break; additional Sponsr shout-outs (3 slides) |
| 2:35 PM | Mark Peters - Integrating DevSecOps Teams |
| 3:00 PM | Secret Speaker - Presy |
| 3:25 PM | Panel Discussion - Unanticipated Dependencies |
| 4:00 PM | Wrap - All Organizers |

</div>

<div markdown="1" style="align-self:flex-start;">
  <img src="/assets/images/duck-dev.png" align="right" style="height:20em;margin-top:2em;" />
  <br />
  <img src="/assets/images/duck-ops.png" align="right" style="height:20em;margin-top:2em;" />
</div>

</div>

{% if site.data.speakers.items.size > 0 %}

# Speakers

{% include speaker-thumbs.html %}

{% endif %}
