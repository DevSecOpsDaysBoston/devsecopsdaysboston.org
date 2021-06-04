---
layout: home
---

# About the Conference

**{{ site.event_short_title }}** is a one-day conference focused on empowering developers, security, and operations practitioners to adopt secure coding and delivery practices, improving how technology and people systems do these things together. It will be held online on July 26th 2021.

100% of net ticket sales and contributor sponsorships will go to good causes [(read more here)](/efforts).

DevSecOps Days is a global series of virtual conferences helping to educate, evolve, and explore concepts around developing security as code.

<div class="flexbox">
  <a class="flexbox-button" href="{{ site.registration.relative_path }}">Attend {{ site.event_short_title }}</a>
  <a class="flexbox-button" href="/sponsor">Sponsor this Event</a>
</div>

# Speakers & Agenda

{% if site.cfp.is_open %}

Our CFP for {{ site.event_short_title }} 2021 is still open until {{ site.cfp.close_date }}!

<div class="flexbox">
  <a class="flexbox-button" href="https://www.papercall.io/devsecops-days-boston-2021">Present Something!</a>
</div>

{% else %}

Our CFP for {{ site.event_short_title }} 2021 closed on {{ site.cfp.close_date }}!
{% if site.data.speakers.items.size < 1 %}
We are currently in the process of reviewing these presentation submissions and will publish the speaker schedule shortly.

{% endif %}
{% endif %}


{% assign items = site.data.sponsors.items | where_exp:"item", "item.level == 'premiere'" %}
{% if items.size > 0 %}

# Premiere Sponsors

These sponsors have materially contributed both in effort and financial underwriting to make this conference possible! A special thanks goes to them for the opportunity to come together and learn!

<div class="flexbox">
  {% for item in items %}
    <a href="{{ item.link }}"><img class="sponsor-logo-{{ item.level }}" src="/assets/images/sponsors/{{ item.logo }}" title="{{ item.name }}"></a>
  {% endfor %}
</div>

{% endif %}

{% assign items = site.data.sponsors.items | where_exp:"item", "item.level == 'contributor'" %}
{% if items.size > 0 %}

# Contributor Sponsors

These sponsors have donated significantly to one of our community-driven 'good causes'.
We can't thank them enough for their support of these worthwhile organizations and this conference!

If you would also like to sponsor in this way, please [contact the organizers](/contact).

<div class="flexbox">
  {% for item in items %}
    <a href="{{ item.link }}"><img class="sponsor-logo-{{ item.level }}" src="/assets/images/sponsors/{{ item.logo }}" title="{{ item.name }}"></a>
  {% endfor %}
</div>

{% endif %}
