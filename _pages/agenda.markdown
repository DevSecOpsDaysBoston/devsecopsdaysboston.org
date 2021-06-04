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

<div class="flexbox" style="">

### Day 1 (7/26)

|   Time   |   Session                         |
| 11:00 AM | Welcome and Intros                |
| 11:15 AM | **Keynote** - TBD |
| 12:00 PM | Sponsored Breakouts |
| 12:20 PM | Speaker / Presentation |
| 1:00 PM  | Speaker / Presentation |
| 1:35 PM  | Sponsored Breakouts |
| 1:55 PM	 | Stretch / Bio Break |
| 2:00 PM  | Speaker / Presentation |
| 2:35 PM  | Speaker / Presentation |
| 2:50 PM  | Contributions Shout-outs          |
| 3:00 PM  | Speaker / Presentation |
| 3:35 PM  | Panel Discussion |
| 4:00 PM  | Day 1 Wrap and Final Reminders    |

</div>

{% if site.data.speakers.items.size > 0 %}

# Speakers

{% include speaker-thumbs.html %}

{% endif %}
