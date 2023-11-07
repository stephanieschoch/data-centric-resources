---
layout: default
title: Outputs
parent: Large Language Models
nav_order: 4
---

# Large Language Model Outputs

Contains papers related to analyzing, evaluating, and utilizing outputs from Large Language Models. 

<!--
For papers related to using LLM outputs for further training (e.g. imitation models), see fine-tuning.
-->

## Large Language Models as Data Generators

### Imitation Models
<details><summary><b>The False Promise of Imitating Proprietary LLMs</b> 
<br>
&emsp;<i>Arnav Gudibande, Eric Wallace, Charlie Snell, Xinyang Geng, Hao Liu, Pieter Abbeel, Sergey Levine, Dawn Song</i>
<br>
&emsp;<i>arXiv, 2023</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2305.15717">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/young-geng/EasyLM">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> An emerging method to cheaply improve a weaker language model is to finetune it on outputs from a stronger model, such as a proprietary system like ChatGPT (e.g., Alpaca, Self-Instruct, and others). This approach looks to cheaply imitate the proprietary model's capabilities using a weaker open-source model. In this work, we critically analyze this approach. We first finetune a series of LMs that imitate ChatGPT using varying base model sizes (1.5B--13B), data sources, and imitation data amounts (0.3M--150M tokens). We then evaluate the models using crowd raters and canonical NLP benchmarks. Initially, we were surprised by the output quality of our imitation models -- they appear far better at following instructions, and crowd workers rate their outputs as competitive with ChatGPT. However, when conducting more targeted automatic evaluations, we find that imitation models close little to none of the gap from the base LM to ChatGPT on tasks that are not heavily supported in the imitation data. We show that these performance discrepancies may slip past human raters because imitation models are adept at mimicking ChatGPT's style but not its factuality. Overall, we conclude that model imitation is a false promise: there exists a substantial capabilities gap between open and closed LMs that, with current methods, can only be bridged using an unwieldy amount of imitation data or by using more capable base LMs. In turn, we argue that the highest leverage action for improving open-source models is to tackle the difficult challenge of developing better base LMs, rather than taking the shortcut of imitating proprietary systems.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{gudibande2023false,
  title={The false promise of imitating proprietary llms},
  author={Gudibande, Arnav and Wallace, Eric and Snell, Charlie and Geng, Xinyang and Liu, Hao and Abbeel, Pieter and Levine, Sergey and Song, Dawn},
  journal={arXiv preprint arXiv:2305.15717},
  year={2023}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>