---
layout: home
title: "{{ site.event_short_title }} {{ site.current_event.dates }}"
---

<div style="clear:both;">
</div>

<div class="flexbox">

<div markdown="1" style="flex:1;align-self:flex-start;">

# It's a Wrap!

To access all the videos:

<ol type="a">
  <li><strong>If you did not already</strong> <a href="/signup">signup, please do so here</a>.</li>
  <li>If you already signed up, please check your email for a Hub invite from hey@vito.community</li>
</ol>

# About the Conference

**{{ site.event_short_title }}** is an ongoing online conference focused on empowering developers, security, and operations practitioners to adopt secure coding and delivery practices, improving how technology and people systems do these things together. It was held on July 26th 2021 but the videos are all available and monthly meetups will follow.

100% of net ticket sales and contributor sponsorships will go to good causes [(read more here)](/efforts).

DevSecOps Days is a global series of virtual conferences helping to educate, evolve, and explore concepts around developing security as code.

</div>

<div class="hide-when-vertical" style="align-self:flex-end;">

  <img src="/assets/images/duck-sec.png" style="height:25em;margin-top:2em;" />

</div>

</div>


<div style="clear:both;">
</div>

<div class="flexbox">
  <a class="flexbox-button" href="{{ site.registration.relative_path }}">Watch {{ site.event_short_title }}</a>
  <a class="flexbox-button" href="/sponsor">Sponsor this Event</a>
</div>

# Speakers & Agenda

{% if site.cfp.is_open %}

  Our CFP for {{ site.event_short_title }} 2021 is still open until {{ site.cfp.close_date }}!

  <div class="flexbox">
    <a class="flexbox-button" href="https://www.papercall.io/devsecops-days-boston-2021">Present Something!</a>
  </div>

{% else %}
  {% if site.data.speakers.items.size < 1 %}

    Our CFP for {{ site.event_short_title }} 2021 closed on {{ site.cfp.close_date }}!

    We are currently in the process of reviewing these presentation submissions and will publish the speaker schedule shortly.
  {% else %}

{% include speaker-thumbs.html %}

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

{% assign items = site.data.sponsors.items | where_exp:"item", "item.level == 'community'" %}
{% if items.size > 0 %}

# Community Sponsors

These sponsors help make all DevSecOps Days events possible!

<div class="flexbox">
  {% for item in items %}
    <a href="{{ item.link }}"><img class="sponsor-logo-{{ item.level }}" src="/assets/images/sponsors/{{ item.logo }}" title="{{ item.name }}"></a>
  {% endfor %}
</div>

{% endif %}
