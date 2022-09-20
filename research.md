---
layout: page
title: "Research & writing"
permalink: /research-writing/
main_nav: true
---

{% for category in site.categories %}
  {% capture cat %}{{ category | first }}{% endcapture %}
  <h2 id="{{cat}}">{{ cat | capitalize }}</h2>
  {% for desc in site.descriptions %}
    {% if desc.cat == cat %}
      <p class="desc"><em>{{ desc.desc }}</em></p>
    {% endif %}
  {% endfor %}
  <ul class="posts-list">
  {% for post in site.categories[cat] %}
    <li>
      <strong>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </strong>
      <span class="post-date">- {{ post.date | date_to_long_string }}</span>
    </li>
  {% endfor %}
  </ul>
  {% if forloop.last == false %}<hr>{% endif %}
{% endfor %}
<br>

<h3>In preparation</h3>
<ol>
  <li>Categorical dynamics on stable module categories</li>
  <li>A HKR-type theorem for real Hochschild homology</li>
</ol>

<h3>Preprint</h3>
<details>
<summary><a href="https://arxiv.org/abs/2008.02821">A descent view on Mitchell's theorem</a> <i>with <a href="https://eldenelmanto.com/">Elden Elmanto</a> and <a href="https://homepages.uni-regensburg.de/~nad22969/">Denis Nardin</a></i></summary>
<i>Abstract:</i> In this short note, we given a new proof of Mitchell's theorem that L<sub>T(n)</sub>K(ℤ)≅0 for n≥2. Instead of reducing the problem to delicate representation theory, we use recently established hyperdescent technology for chromatically-localized algebraic K-theory.
</details>


<h3>Other</h3>

A copy of my minor thesis can be found [here]({{site.baseurl}}/assets/LYang%20minor%20thesis.pdf). 