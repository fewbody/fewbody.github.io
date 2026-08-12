---
title: "Gallery - QFBD Research Group"
layout: textlay
excerpt: "Photos of the Quantum Few-Body Dynamics Group, Tongji University."
sitemap: false
permalink: /gallery/
---

<h1><span class="l-en">Gallery</span><span class="l-zh">相册</span></h1>

<p class="lede l-en">Visitors, conferences, and exchange visits, most recent first.</p>
<p class="lede l-zh">来访学者、学术会议与出访交流的照片，按时间倒序排列。</p>

{::nomarkdown}
<div class="photo-grid">
{% for pic in site.data.gallery %}
<figure class="photo-card">
<a href="{{ site.url }}{{ site.baseurl }}/images/grouppic/{{ pic.image }}"><img src="{{ site.url }}{{ site.baseurl }}/images/grouppic/{{ pic.image }}" alt="{{ pic.caption }}" loading="lazy" /></a>
<figcaption><span class="l-en">{{ pic.caption }}</span><span class="l-zh">{{ pic.caption_zh }}</span></figcaption>
</figure>
{% endfor %}
</div>
{:/nomarkdown}
