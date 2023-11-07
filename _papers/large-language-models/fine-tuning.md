---
layout: default
title: Fine-tuning 
parent: Large Language Models
nav_order: 2
---

### 2023
<details><summary><b>An Emulator for Fine-Tuning Large Language Models using Small Language Models</b> <br>
&emsp;<i>Eric Mitchell, Rafael Rafailov, Archit Sharma, Chelsea Finn, Christopher D. Manning</i><br>
&emsp;<i>arXiv, 2023</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2310.12962">Paper</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> Widely used language models (LMs) are typically built by scaling up a two-stage training pipeline: a pre-training stage that uses a very large, diverse dataset of text and a fine-tuning (sometimes, 'alignment') stage that uses targeted examples or other specifications of desired behaviors. While it has been hypothesized that knowledge and skills come from pre-training, and fine-tuning mostly filters this knowledge and skillset, this intuition has not been extensively tested. To aid in doing so, we introduce a novel technique for decoupling the knowledge and skills gained in these two stages, enabling a direct answer to the question, "What would happen if we combined the knowledge learned by a large model during pre-training with the knowledge learned by a small model during fine-tuning (or vice versa)?" Using an RL-based framework derived from recent developments in learning from human preferences, we introduce emulated fine-tuning (EFT), a principled and practical method for sampling from a distribution that approximates (or 'emulates') the result of pre-training and fine-tuning at different scales. Our experiments with EFT show that scaling up fine-tuning tends to improve helpfulness, while scaling up pre-training tends to improve factuality. Beyond decoupling scale, we show that EFT enables test-time adjustment of competing behavioral traits like helpfulness and harmlessness without additional training. Finally, a special case of emulated fine-tuning, which we call LM up-scaling, avoids resource-intensive fine-tuning of large pre-trained models by ensembling them with small fine-tuned models, essentially emulating the result of fine-tuning the large pre-trained model. Up-scaling consistently improves helpfulness and factuality of instruction-following models in the Llama, Llama-2, and Falcon families, without additional hyperparameters or training.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{mitchell2023emulator,
  title={An Emulator for Fine-Tuning Large Language Models using Small Language Models},
  author={Mitchell, Eric and Rafailov, Rafael and Sharma, Archit and Finn, Chelsea and Manning, Christopher D},
  journal={arXiv preprint arXiv:2310.12962},
  year={2023}
}</code></pre>
{% endraw %}
</details>

</blockquote></details>

<details><summary><b>LIMA: Less Is More for Alignment</b> 
<br>
&emsp;<i>Chunting Zhou, Pengfei Liu, Puxin Xu, Srini Iyer, Jiao Sun, Yuning Mao, Xuezhe Ma, Avia Efrat, Ping Yu, Lili Yu, Susan Zhang, Gargi Ghosh, Mike Lewis, Luke Zettlemoyer, Omer Levy</i>
<br>
&emsp;<i>arXiv, 2023</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2305.11206">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Large language models are trained in two stages: (1) unsupervised pretraining from raw text, to learn general-purpose representations, and (2) large scale instruction tuning and reinforcement learning, to better align to end tasks and user preferences. We measure the relative importance of these two stages by training LIMA, a 65B parameter LLaMa language model fine-tuned with the standard supervised loss on only 1,000 carefully curated prompts and responses, without any reinforcement learning or human preference modeling. LIMA demonstrates remarkably strong performance, learning to follow specific response formats from only a handful of examples in the training data, including complex queries that range from planning trip itineraries to speculating about alternate history. Moreover, the model tends to generalize well to unseen tasks that did not appear in the training data. In a controlled human study, responses from LIMA are either equivalent or strictly preferred to GPT-4 in 43% of cases; this statistic is as high as 58% when compared to Bard and 65% versus DaVinci003, which was trained with human feedback. Taken together, these results strongly suggest that almost all knowledge in large language models is learned during pretraining, and only limited instruction tuning data is necessary to teach models to produce high quality output.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{zhou2023lima,
  title={Lima: Less is more for alignment},
  author={Zhou, Chunting and Liu, Pengfei and Xu, Puxin and Iyer, Srini and Sun, Jiao and Mao, Yuning and Ma, Xuezhe and Efrat, Avia and Yu, Ping and Yu, Lili and others},
  journal={arXiv preprint arXiv:2305.11206},
  year={2023}
}
</code></pre>
{% endraw %}
</details>
</blockquote>
</details>
