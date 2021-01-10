---
layout: page
title: 檔案下載
permalink: /download/
---

## 手冊
{% assign manu = site.static_files | where: "manual", true %}
{% for m in manu %}
  [{{ m.basename }}]({{m.path}})
{% endfor %}

## 歷屆考題
[全部下載](/assets/cpge_annals.zip)
{% assign annals = site.static_files | where: "annal", true | reverse %}
{% for annal in annals %}
  <span class="col-md-4">[{{ annal.basename }}]({{annal.path}})</span>
{% endfor %}

## Brief Correction
{% assign corr = site.static_files | where: "correct", true | reverse %}
{% for c in corr %}
  <span class="col-md-4">[{{ c.basename }}]({{c.path}})</span>
{% endfor %}

