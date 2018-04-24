---
layout: page
title: About
description: lkJack的个人博客
keywords: lkJack, luckydogJack
comments: true
menu: 关于
permalink: /about/
---

Luckydogjack

a student from scut

try to share with the world.

## 联系

{% for website in site.data.social %}
* {{ website.sitename }}：[@{{ website.name }}]({{ website.url }})
{% endfor %}

## Skill Keywords

{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
