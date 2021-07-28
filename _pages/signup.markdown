---
layout: default
title:  "Watch {{ site.event_short_title }}"
permalink: /signup
---

<div class="flexbox">

  <div style="flex:1;align-self:flex-start;min-width:600px;padding-right:2em;">

    <div markdown=1>

# Get access to our hub!

If you haven't registered yet for access, please use the options below. Remember
 to do a good thing for others if you can by donating, but if you can't just uncheck
 the donate option and check the free one instead.

</div>
<link rel="stylesheet" type="text/css" href='https://css.tito.io/v1.1' />
<style type="text/css">
.tito-badge-link {
  display: none;
  visibility: hidden;
}
.tito-wrapper {
  color: #eee;
}
* {
  box-sizing: content-box;
}
</style>

<script src='https://js.tito.io/v1' async></script>

<tito-widget event="devsecops-days-boston/2021"></tito-widget>

</div>
<div style="flex:1;align-self:flex-start;min-width:200px;" markdown=1>

# Already registered?

Look for an email like the one below from 'hey@vito.community'. Don't forget
 to check your junk/spam folders.

<img src="/assets/images/sample-hub-invite.jpg" style="width:100%;" />

</div>
</div>

***Once you are registered and signed in to the hub***, [you can access it here.](https://vi.to/hubs/devsecops-days-boston-2021/pages/videos)

<div class="flexbox">

<div style="flex:1;align-self:flex-start;min-width:400px;padding-right:2em;" markdown=1>

# Why Donate for Charity?

As a single contributor, you can make a difference, and we all should. As a group,
 we can make a significant collective difference for some really good causes:

<div style="font-size:0.8em;" markdown=1>

{% include good-cause-list.html %}

</div>

</div>
<div style="flex:1;align-self:flex-start;min-width:400px;" markdown=1>

# Logistics

This event was held online on July 26th and was live captioned to respect accessibility for all attendees. It
 is also be accessible via mobile device and standard desktop browsers (the after-party platform
 is only for full browsers).

</div>

<div style="text-align:left;">
<h1>Who was there?</h1>
<p>
Hundreds of other community members and engineering folks will be online listening to,
 discussing with, and learning from each other about security practices.
</p>
{% if site.data.speakers.items.size > 0 %}
<p>
Oh, and did we mention an ***amazing*** lineup of speakers, open source contributors,
 and practitioners already implementing advanced security practices in their
 organizations? Check out some of them below:
</p>
{% endif %}
</div>

{% if site.data.speakers.items.size > 0 %}
{% include speaker-thumbs.html %}
{% endif %}
