---
layout: default
title: Shapley Applications
parent: Shapley Values
grand_parent: Data Contribution Estimation
nav_order: 3
---
## Applications of Shapley-based Data Contribution Estimation

### 2023

<details><summary><b>Data Selection for Fine-tuning Large Language Models Using Transferred Shapley Values</b> 
<br>
&emsp;<i>Stephanie Schoch, Ritwick Mishra, Yangfeng Ji</i>
<br>
&emsp;<i>Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 4: Student Research Workshop), 2023</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://aclanthology.org/2023.acl-srw.37/">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/stephanieschoch/ts-dshapley">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Although Shapley values have been shown to be highly effective for identifying harmful training instances, dataset size and model complexity constraints limit the ability to apply Shapley-based data valuation to fine-tuning large pre-trained language models. To address this, we propose TS-DShapley, an algorithm that reduces computational cost of Shapley-based data valuation through: 1) an efficient sampling-based method that aggregates Shapley values computed from subsets for valuation of the entire training set, and 2) a value transfer method that leverages value information extracted from a simple classifier trained using representations from the target language model. Our experiments applying TS-DShapley to select data for fine-tuning BERT-based language models on benchmark natural language understanding (NLU) datasets show that TS-DShapley outperforms existing data selection methods. Further, TS-DShapley can filter fine-tuning data to increase language model performance compared to training with the full fine-tuning dataset.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @inproceedings{schoch-etal-2023-data,
    title = "Data Selection for Fine-tuning Large Language Models Using Transferred Shapley Values",
    author = "Schoch, Stephanie  and
      Mishra, Ritwick  and
      Ji, Yangfeng",
    editor = "Padmakumar, Vishakh  and
      Vallejo, Gisela  and
      Fu, Yao",
    booktitle = "Proceedings of the 61st Annual Meeting of the Association for Computational Linguistics (Volume 4: Student Research Workshop)",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.acl-srw.37",
    doi = "10.18653/v1/2023.acl-srw.37",
    pages = "266--275"
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


### 2021

<details><summary><b>Data valuation for medical imaging using Shapley value and application to a large-scale chest X-ray dataset</b> 
<br>
&emsp;<i>Siyi Tang, Amirata Ghorbani, Rikiya Yamashita, Sameer Rehman, Jared A. Dunnmon, James Zou & Daniel L. Rubin</i>
<br>
&emsp;<i>Nature Scientific Reports, 2021</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://www.nature.com/articles/s41598-021-87762-2">Paper</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> The reliability of machine learning models can be compromised when trained on low quality data. Many large-scale medical imaging datasets contain low quality labels extracted from sources such as medical reports. Moreover, images within a dataset may have heterogeneous quality due to artifacts and biases arising from equipment or measurement errors. Therefore, algorithms that can automatically identify low quality data are highly desired. In this study, we used data Shapley, a data valuation metric, to quantify the value of training data to the performance of a pneumonia detection algorithm in a large chest X-ray dataset. We characterized the effectiveness of data Shapley in identifying low quality versus valuable data for pneumonia detection. We found that removing training data with high Shapley values decreased the pneumonia detection performance, whereas removing data with low Shapley values improved the model performance. Furthermore, there were more mislabeled examples in low Shapley value data and more true pneumonia cases in high Shapley value data. Our results suggest that low Shapley value indicates mislabeled or poor quality images, whereas high Shapley value indicates data that are valuable for pneumonia detection. Our method can serve as a framework for using data Shapley to denoise large-scale medical imaging datasets.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{tang2021data,
  title={Data valuation for medical imaging using Shapley value and application to a large-scale chest X-ray dataset},
  author={Tang, Siyi and Ghorbani, Amirata and Yamashita, Rikiya and Rehman, Sameer and Dunnmon, Jared A and Zou, James and Rubin, Daniel L},
  journal={Scientific reports},
  volume={11},
  number={1},
  pages={8366},
  year={2021},
  publisher={Nature Publishing Group UK London}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


### 2020

<details><summary><b>A Principled Approach to Data Valuation for Federated Learning</b> <br>
&emsp;<i>Tianhao Wang, Johannes Rausch, Ce Zhang, Ruoxi Jia, Dawn Song</i><br>
&emsp;<i>Federated Learning: Privacy and Incentive, 2020</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2009.06192">Paper</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> Federated learning (FL) is a popular technique to train machine learning (ML) models on decentralized data sources. In order to sustain long-term participation of data owners, it is important to fairly appraise each data source and compensate data owners for their contribution to the training process. The Shapley value (SV) defines a unique payoff scheme that satisfies many desiderata for a data value notion. It has been increasingly used for valuing training data in centralized learning. However, computing the SV requires exhaustively evaluating the model performance on every subset of data sources, which incurs prohibitive communication cost in the federated setting. Besides, the canonical SV ignores the order of data sources during training, which conflicts with the sequential nature of FL. This paper proposes a variant of the SV amenable to FL, which we call the federated Shapley value. The federated SV preserves the desirable properties of the canonical SV while it can be calculated without incurring extra communication cost and is also able to capture the effect of participation order on data value. We conduct a thorough empirical study of the federated SV on a range of tasks, including noisy label detection, adversarial participant detection, and data summarization on different benchmark datasets, and demonstrate that it can reflect the real utility of data sources for FL and has the potential to enhance system robustness, security, and efficiency. We also report and analyze "failure cases" and hope to stimulate future research.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{wang2020principled,
  title={A principled approach to data valuation for federated learning},
  author={Wang, Tianhao and Rausch, Johannes and Zhang, Ce and Jia, Ruoxi and Song, Dawn},
  journal={Federated Learning: Privacy and Incentive},
  pages={153--167},
  year={2020},
  publisher={Springer}
} </code></pre>
{% endraw %}
</details>
</blockquote></details>