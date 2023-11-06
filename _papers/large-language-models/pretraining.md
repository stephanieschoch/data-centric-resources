---
layout: default
title: Pretraining
parent: Large Language Models
nav_order: 2
---

## Pretraininig Data

<details><summary><b>Detecting Pretraining Data from Large Language Models</b> 
<br>
&emsp;<i>Weijia Shi, Anirudh Ajith, Mengzhou Xia, Yangsibo Huang, Daogao Liu, Terra Blevins, Danqi Chen, Luke Zettlemoyer</i>
<br>
&emsp;<i>arXiv, 2023</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2310.16789">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/swj0419/detect-pretrain-code">Code</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://swj0419.github.io/detect-pretrain.github.io/">Blog</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://huggingface.co/datasets/swj0419/WikiMIA">Dataset</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Although large language models (LLMs) are widely deployed, the data used to train them is rarely disclosed. Given the incredible scale of this data, up to trillions of tokens, it is all but certain that it includes potentially problematic text such as copyrighted materials, personally identifiable information, and test data for widely reported reference benchmarks. However, we currently have no way to know which data of these types is included or in what proportions. In this paper, we study the pretraining data detection problem: given a piece of text and black-box access to an LLM without knowing the pretraining data, can we determine if the model was trained on the provided text? To facilitate this study, we introduce a dynamic benchmark WIKIMIA that uses data created before and after model training to support gold truth detection. We also introduce a new detection method Min-K% Prob based on a simple hypothesis: an unseen example is likely to contain a few outlier words with low probabilities under the LLM, while a seen example is less likely to have words with such low probabilities. Min-K% Prob can be applied without any knowledge about the pretraining corpus or any additional training, departing from previous detection methods that require training a reference model on data that is similar to the pretraining data. Moreover, our experiments demonstrate that Min-K% Prob achieves a 7.4% improvement on WIKIMIA over these previous methods. We apply Min-K% Prob to two real-world scenarios, copyrighted book detection, and contaminated downstream example detection, and find it a consistently effective solution.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{shi2023detecting,
  title={Detecting Pretraining Data from Large Language Models},
  author={Shi, Weijia and Ajith, Anirudh and Xia, Mengzhou and Huang, Yangsibo and Liu, Daogao and Blevins, Terra and Chen, Danqi and Zettlemoyer, Luke},
  journal={arXiv preprint arXiv:2310.16789},
  year={2023}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>

