---
layout: page
title: 聯絡我們
permalink: /contact
---

{% for contact in site.data.contacts %}
  * {{contact.name}} ({{contact.highschool}}/{{contact.prepa}}/{{contact.grandeecole}})

    {{contact.email}}
{% endfor %}
