---
layout: default
title: Model Evaluation
parent: Large Language Models
nav_order: 5
---

# Evaluating LLMs using Data-Centric Methods

<details><summary><b>We're Afraid Language Models Aren't Modeling Ambiguity</b> <br>
&emsp;<i>Alisa Liu, Zhaofeng Wu, Julian Michael, Alane Suhr, Peter West, Alexander Koller, Swabha Swayamdipta, Noah A. Smith, Yejin Choi</i><br>
&emsp;<i>arXiv, 2023 (Accepted to EMNLP 2023)</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2304.14399">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/alisawuffles/ambient">Data & Code</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> Ambiguity is an intrinsic feature of natural language. Managing ambiguity is a key part of human language understanding, allowing us to anticipate misunderstanding as communicators and revise our interpretations as listeners. As language models (LMs) are increasingly employed as dialogue interfaces and writing aids, handling ambiguous language is critical to their success. We characterize ambiguity in a sentence by its effect on entailment relations with another sentence, and collect AmbiEnt, a linguist-annotated benchmark of 1,645 examples with diverse kinds of ambiguity. We design a suite of tests based on AmbiEnt, presenting the first evaluation of pretrained LMs to recognize ambiguity and disentangle possible meanings. We find that the task remains extremely challenging, including for GPT-4, whose generated disambiguations are considered correct only 32% of the time in human evaluation, compared to 90% for disambiguations in our dataset. Finally, to illustrate the value of ambiguity-sensitive tools, we show that a multilabel NLI model can flag political claims in the wild that are misleading due to ambiguity. We encourage the field to rediscover the importance of ambiguity for NLP.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{liu2023we,
  title={We're Afraid Language Models Aren't Modeling Ambiguity},
  author={Liu, Alisa and Wu, Zhaofeng and Michael, Julian and Suhr, Alane and West, Peter and Koller, Alexander and Swayamdipta, Swabha and Smith, Noah A and Choi, Yejin},
  journal={arXiv preprint arXiv:2304.14399},
  year={2023}
} </code></pre>
{% endraw %}
</details>
</blockquote></details>