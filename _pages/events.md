---
layout: page
permalink: /events/
title: Events
description: 
nav: false
nav_order: 5
---
Subscribe to our mailing list [here](https://lists.lrz.de/mailman/listinfo/lmu-cis-mainlp-events).
<!-- pages/events.md -->
<!-- events are sorted by filename (reverse order) -->
<div class="events">
  {%- for event in site.events reversed -%}
    <div class="event">
	  {% include events.html %}
    </div>
  {%- endfor %}
</div>