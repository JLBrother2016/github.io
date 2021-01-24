---
layout: page
title: About
description: 知其然而必知其所以然，深度思考
keywords: jlcoo, 蒋龙
comments: true
menu: 关于
permalink: /about/
---

明日复明日，明日何其多？日日待明日，万事成蹉跎。 ——（明·文嘉）

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
</ul>

## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
