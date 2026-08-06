---
title: "Team - QFBD Research Group"
layout: gridlay
excerpt: "Members of the Quantum Few-Body Dynamics Group, Tongji University."
sitemap: false
permalink: /team/
---

<div markdown="0">

<h1><span class="l-en">Group members</span><span class="l-zh">课题组成员</span></h1>

<h2><span class="l-en">Faculty</span><span class="l-zh">教师</span></h2>

<div class="member-grid">
{% for member in site.data.team_members %}
  <div class="member">
    <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="member-photo" alt="{{ member.name | strip_html }}" />
    <div class="member-body">
      <h4><span class="l-en">{{ member.name }}</span><span class="l-zh">{% if member.name_zh %}{{ member.name_zh }}{% else %}{{ member.name }}{% endif %}</span></h4>
      <p><span class="l-en">{{ member.info }}</span><span class="l-zh">{% if member.info_zh %}{{ member.info_zh }}{% else %}{{ member.info }}{% endif %}</span></p>
      {% if member.number_educ and member.number_educ > 0 %}
      <ul>
        {% for i in (1..member.number_educ) %}
          {% assign key = 'education' | append: i %}
          {% if member[key] %}<li>{{ member[key] }}</li>{% endif %}
        {% endfor %}
      </ul>
      {% endif %}
      {% if member.email %}<p class="member-mail"><a href="mailto:{{ member.email }}">{{ member.email }}</a></p>{% endif %}
    </div>
  </div>
{% endfor %}
</div>

<h2><span class="l-en">PhD and master's students</span><span class="l-zh">博士与硕士研究生</span></h2>

<div class="member-grid">
{% for member in site.data.students %}
  <div class="member">
    <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="member-photo" alt="{{ member.name | strip_html }}" />
    <div class="member-body">
      <h4><span class="l-en">{{ member.name }}</span><span class="l-zh">{% if member.name_zh %}{{ member.name_zh }}{% else %}{{ member.name }}{% endif %}</span></h4>
      <p><span class="l-en">{{ member.info }}</span><span class="l-zh">{% if member.info_zh %}{{ member.info_zh }}{% else %}{{ member.info }}{% endif %}</span></p>
    </div>
  </div>
{% endfor %}
</div>

<h2><span class="l-en">Alumni</span><span class="l-zh">已毕业成员</span></h2>

<div class="member-grid">
{% for member in site.data.alumni_members %}
  <div class="member">
    <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="member-photo" alt="{{ member.name | strip_html }}" />
    <div class="member-body">
      <h4><span class="l-en">{{ member.name }}</span><span class="l-zh">{% if member.name_zh %}{{ member.name_zh }}{% else %}{{ member.name }}{% endif %}</span></h4>
      {% if member.duration %}<p class="member-role"><span class="l-en">{{ member.duration }}</span><span class="l-zh">{% if member.duration_zh %}{{ member.duration_zh }}{% else %}{{ member.duration }}{% endif %}</span></p>{% endif %}
      <p><span class="l-en">{{ member.info }}</span><span class="l-zh">{% if member.info_zh %}{{ member.info_zh }}{% else %}{{ member.info }}{% endif %}</span></p>
    </div>
  </div>
{% endfor %}
</div>

</div>
