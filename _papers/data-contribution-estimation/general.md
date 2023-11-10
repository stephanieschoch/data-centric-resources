---
layout: default
title: General (e.g. Surveys)
parent: Data Contribution Estimation
nav_order: 4
has_children: false
---

## General (e.g. Surveys)

<details><summary><b>Data Valuation in Machine Learning: “Ingredients”, Strategies, and Open Challenges</b> 
<br>
&emsp;<i>Rachael Hwee Ling Sim, Xinyi Xu, Bryan Kian Hsiang Low</i>
<br>
&emsp;<i>Proceedings of the Thirty-First International Joint Conference on Artificial Intelligence
Survey Track (IJCAI), 2022</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://www.ijcai.org/proceedings/2022/782">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://www.ijcai.org/proceedings/2022/video/782">Video</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Data valuation in machine learning (ML) is an emerging research area that studies the worth of data in ML. Data valuation is used in collaborative ML to determine a fair compensation for every data owner and in interpretable ML to identify the most responsible, noisy, or misleading training examples. This paper presents a comprehensive technical survey that provides a new formal study of data valuation in ML through its “ingredients” and the corresponding properties, grounds the discussion of common desiderata satisfied by existing data valuation strategies on our proposed ingredients, and identifies open research challenges for designing new ingredients, data valuation strategies, and cost reduction techniques.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @inproceedings{sim2022data,
  title={Data valuation in machine learning:“ingredients”, strategies, and open challenges},
  author={Sim, Rachael Hwee Ling and Xu, Xinyi and Low, Bryan Kian Hsiang},
  booktitle={Proc. IJCAI},
  pages={5607--5614},
  year={2022}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>

<details><summary><b>Training Data Influence Analysis and Estimation: A Survey</b> <br>
&emsp;<i>Zayd Hammoudeh, Daniel Lowd</i><br>
&emsp;<i>arXiv. 2022</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2212.04612">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/ZaydH/influence_analysis_papers">Repository</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> Good models require good training data. For overparameterized deep models, the causal relationship between training data and model predictions is increasingly opaque and poorly understood. Influence analysis partially demystifies training's underlying interactions by quantifying the amount each training instance alters the final model. Measuring the training data's influence exactly can be provably hard in the worst case; this has led to the development and use of influence estimators, which only approximate the true influence. This paper provides the first comprehensive survey of training data influence analysis and estimation. We begin by formalizing the various, and in places orthogonal, definitions of training data influence. We then organize state-of-the-art influence analysis methods into a taxonomy; we describe each of these methods in detail and compare their underlying assumptions, asymptotic complexities, and overall strengths and weaknesses. Finally, we propose future research directions to make influence analysis more useful in practice as well as more theoretically and empirically sound. A curated, up-to-date list of resources related to influence analysis is available at this https URL.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{Hammoudeh:2022:InfluenceSurvey,
  author = {Zayd Hammoudeh and 
            Daniel Lowd},
  title = {Training Data Influence Analysis and Estimation: A Survey},
  archivePrefix = {arXiv},
  eprint = {2212.04612},
  primaryClass = {cs.LG},
  year = {2022},
} </code></pre>
{% endraw %}
</details>
</blockquote></details>


<details><summary><b>Energy-Based Learning for Cooperative Games, with Applications to Valuation Problems in Machine Learning</b> <br>
&emsp;<i>Yatao Bian, Yu Rong, Tingyang Xu, Jiaxiang Wu, Andreas Krause, Junzhou Huang</i><br>
&emsp;<i>International Conference on Learning Representations (ICLR), 2022</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://openreview.net/forum?id=xLfAgCroImw">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/tencent-ailab/valuationgame">Code</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://iclr.cc/virtual/2022/poster/6807">Talk</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://yataobian.com/docs/val-game-poster-v2.png">Poster</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://yataobian.com/docs/valuation-game-slides-v3.pdf">Slides</a>]

<br><br></summary>

<blockquote> <b>Abstract:</b> Valuation problems, such as feature interpretation, data valuation and model valuation for ensembles, become increasingly more important in many machine learning applications. Such problems are commonly solved by well-known game-theoretic criteria, such as Shapley value or Banzhaf value. In this work, we present a novel energy-based treatment for cooperative games, with a theoretical justification by the maximum entropy framework. Surprisingly, by conducting variational inference of the energy-based model, we recover various game-theoretic valuation criteria through conducting one-step fixed point iteration  for maximizing the mean-field ELBO objective. This observation also verifies the rationality of existing criteria, as they are all attempting to  decouple the  correlations  among  the  players  through the  mean-field approach. By running fixed point iteration for multiple steps, we achieve a trajectory of the valuations, among which we define the valuation with the best conceivable decoupling error as the Variational Index. We prove that under uniform initializations,  these variational valuations all satisfy a set of game-theoretic axioms. We experimentally demonstrate that the proposed Variational Index enjoys lower decoupling error and better valuation performance  on certain synthetic and real-world valuation problems.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @inproceedings{
bian2022energybased,
title={Energy-Based Learning for Cooperative Games, with Applications to Valuation Problems in Machine Learning},
author={Yatao Bian and Yu Rong and Tingyang Xu and Jiaxiang Wu and Andreas Krause and Junzhou Huang},
booktitle={International Conference on Learning Representations},
year={2022},
url={https://openreview.net/forum?id=xLfAgCroImw}
} </code></pre>
{% endraw %}
</details>
</blockquote></details>


<details><summary><b>Improving Cooperative Game Theory-based Data Valuation via Data Utility Learning</b> <br>
&emsp;<i>Tianhao Wang, Yu Yang, Ruoxi Jia</i><br>
&emsp;<i>ICLR 2022 Workshop on Socially Responsible Machine Learning (SRML), 2022</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2107.06336">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://tianhaowang.netlify.app/pdf/iclrworkshop-poster.pdf">Poster</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> The Shapley value (SV) and Least core (LC) are classic methods in cooperative game theory for cost/profit sharing problems. Both methods have recently been proposed as a principled solution for data valuation tasks, i.e., quantifying the contribution of individual datum in machine learning. However, both SV and LC suffer computational challenges due to the need for retraining models on combinatorially many data subsets. In this work, we propose to boost the efficiency in computing Shapley value or Least core by learning to estimate the performance of a learning algorithm on unseen data combinations. Theoretically, we derive bounds relating the error in the predicted learning performance to the approximation error in SV and LC. Empirically, we show that the proposed method can significantly improve the accuracy of SV and LC estimation.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{wang2021improving,
  title={Improving cooperative game theory-based data valuation via data utility learning},
  author={Wang, Tianhao and Yang, Yu and Jia, Ruoxi},
  journal={ICLR Workshop on Socially Responsible Machine Learning},
  year={2022}
} </code></pre>
{% endraw %}
</details>
</blockquote></details>