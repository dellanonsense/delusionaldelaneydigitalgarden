---
layout: page
title: Home
id: home
permalink: /
---

# welcome, sweetheart, to the trainwreck 

erleww!!


<img src="https://pbs.twimg.com/profile_banners/3090091229/1677104303/600x200">

<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
