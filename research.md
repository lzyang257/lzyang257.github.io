---
layout: page
title: "Research & writing"
permalink: /research-writing/
main_nav: true 
use_math: true
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
  <li>A HKR-type theorem for real Hochschild homology</li>
</ol>

<h3>Preprints</h3>
<details>
<summary> <a href="{{site.baseurl}}/assets/normedrings.pdf">On normed $ \mathbb{E}_\infty $-rings in genuine equivariant $ C_p $-spectra</a>  (last updated August 2023)</summary>
<p class="abstract"><i>Abstract:</i>  Genuine equivariant homotopy theory is equipped with a multitude of coherently commutative multiplication structures generalizing the classical notion of an $ \mathbb{E}_\infty $-algebra. In this paper we study the $ C_p $-$ \mathbb{E}_\infty $-algebras of Nardin--Shah with respect to a cyclic group $ C_p $ of prime power order. We show that many of the higher coherences inherent to the definition of parametrized algebras collapse; in particular, they may be described more simply and conceptually in terms of ordinary $ \mathbb{E}_\infty $-algebras as a diagram category which we call \emph{normed algebras}. 
Our main result provides a relatively straightforward criterion for identifying $ C_p $-$ \mathbb{E}_\infty $-algebra structures. 
We visit some applications of our result to real motivic invariants.  </p>
</details>
<details>
<summary><a href="https://arxiv.org/abs/2212.09964">Categorical dynamics on stable module categories</a> (last updated December 2022)</summary>
<p class="abstract"><i>Abstract:</i>  Let <i>A</i> be a finite connected graded cocommutative Hopf algebra over a field <i>k</i>.  
  There is an endofunctor <tt>tw</tt> on the stable module category StMod<sub>A</sub> of <i>A</i> which twists the grading by 1. 
  We show the categorical entropy of <tt>tw</tt> is zero.
  We provide a lower bound for the categorical polynomial entropy of <tt>tw</tt> in terms of the Krull dimension of the cohomology of <i>A</i>, and an upper bound in terms of the existence of finite resolutions of <i>A</i>-modules of a particular form. 
  We employ these tools to compute the categorical polynomial entropy of the twist functor for examples of finite graded Hopf algebras over $\mathbb{F}$<sub>2</sub>. </p>
</details>
<details>
<summary><a href="https://arxiv.org/abs/2008.02821">A descent view on Mitchell's theorem</a> <i>with <a href="https://eldenelmanto.com/">Elden Elmanto</a> and <a href="https://homepages.uni-regensburg.de/~nad22969/">Denis Nardin</a></i></summary>
<p class="abstract"><i>Abstract:</i> In this short note, we given a new proof of Mitchell's theorem that $L_{T(n)}K(\mathbb{Z}) \simeq 0$ for $n \geq 2$. Instead of reducing the problem to delicate representation theory, we use recently established hyperdescent technology for chromatically-localized algebraic K-theory.</p>
</details>


<h3>Other</h3>

A copy of my minor thesis can be found [here]({{site.baseurl}}/assets/LYang%20minor%20thesis.pdf). 