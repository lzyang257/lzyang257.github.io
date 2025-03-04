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

<h3>Preprints</h3>
<details>
<summary> <a href="{{site.baseurl}}/assets/filtered_HKR_for_HR.pdf">A filtered Hochschild-Kostant-Rosenberg theorem for real Hochschild homology</a>  (last updated March 2025)</summary>
  <p class="abstract"><i>Abstract:</i>  In this paper, we introduce a notion of derived involutive algebras in $ C_2 $-Mackey functors which simultaneously generalize commutative rings with involution and the (non-equivariant) derived algebras of Bhatt--Mathew and Raksit. 
  We show that the $ \infty $-category of derived involutive algebras admits involutive enhancements of the cotangent complexes, de Rham complex, and de Rham cohomology functors; furthermore, their real Hochschild homology is defined. 
  We identify a filtration on the real Hochschild homology of these derived involutive algebras via a universal property and show that its associated graded may be identified with the involutive de Rham complex. 
  Using $ C_2 $-$ \infty $-categories of Barwick--Dotto--Glasman--Nardin--Shah, we show that our filtered real Hochschild homology specializes to the HKR-filtered Hochschild homology considered by Raksit.    </p>
</details>
<details>
<summary><a href="https://arxiv.org/abs/2409.05965">Equivariant Witt Complexes and Twisted Topological Hochschild Homology
</a></summary>
<p class="abstract"><i>Abstract:</i>  The topological Hochschild homology of a ring (or ring spectrum) R is an $S^1$-spectrum, and the fixed points of THH(R) for subgroups $C_n \subset S^1$ have been widely studied due to their use in algebraic K-theory computations. Hesselholt and Madsen proved that the fixed points of topological Hochschild homology are closely related to Witt vectors. Further, they defined the notion of a Witt complex, and showed that it captures the algebraic structure of the homotopy groups of the fixed points of THH. Recent work of Angeltveit, Blumberg, Gerhardt, Hill, Lawson and Mandell defines a theory of twisted topological Hochschild homology for equivariant rings (or ring spectra) that builds upon Hill, Hopkins and Ravenel's work on equivariant norms. In this paper, we study the algebraic structure of the equivariant homotopy groups of twisted THH. In particular, we define an equivariant Witt complex and prove that the equivariant homotopy of twisted THH has this structure. Our definition of equivariant Witt complexes contributes to a growing body of research in the subject of equivariant algebra. </p>
</details>
<details>
<summary> <a href="{{site.baseurl}}/assets/normedrings.pdf">On normed $ \mathbb{E}_\infty $-rings in genuine equivariant $ C_p $-spectra</a>  (last updated July 2024)</summary>
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