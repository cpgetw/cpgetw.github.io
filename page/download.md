---
layout: page
title: 檔案下載
permalink: /download/
---

## 歷屆考題
[全部下載](/assets/cpge_annals.zip)
{% assign annals = site.static_files | where: "annal", true %}
{% for annal in annals %}
  [{{ annal.basename }}]({{annal.path}})
{% endfor %}

## Brief Correction
{% assign cool = site.static_files | where: "_c", true %}
{% for annal in cool %}
  [{{ annal.basename }}]({{annal.path}})
{% endfor %}
