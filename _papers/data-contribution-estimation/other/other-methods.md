---
layout: page
title: Other Methods
parent: Other Approaches
grand_parent: Data Contribution Estimation
nav_order: 2
---

## Other Methods for Data Contribution Estimation
{: .no_toc }

<!--
## Table of contents
{: .no_toc .text-delta }
-->

<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>


<details><summary><b>DAVINZ: Data Valuation using Deep Neural Networks at Initialization</b> 
<br>
&emsp;<i>Zhaoxuan Wu, Yao Shu, Bryan Kian Hsiang Low</i>
<br>
&emsp;<i>Proceedings of the 39th International Conference on Machine Learning (ICML), 2022</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.mlr.press/v162/wu22j.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://icml.cc/media/icml-2022/Slides/17500.pdf">Slides</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Recent years have witnessed a surge of interest in developing trustworthy methods to evaluate the value of data in many real-world applications (e.g., collaborative machine learning, data marketplaces). Existing data valuation methods typically valuate data using the generalization performance of converged machine learning models after their long-term model training, hence making data valuation on large complex deep neural networks (DNNs) unaffordable. To this end, we theoretically derive a domain-aware generalization bound to estimate the generalization performance of DNNs without model training. We then exploit this theoretically derived generalization bound to develop a novel training-free data valuation method named data valuation at initialization (DAVINZ) on DNNs, which consistently achieves remarkable effectiveness and efficiency in practice. Moreover, our training-free DAVINZ, surprisingly, can even theoretically and empirically enjoy the desirable properties that training-based data valuation methods usually attain, thus making it more trustworthy in practice.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

### 2022

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> 
@InProceedings{pmlr-v162-wu22j,
  title = 	 {{DAVINZ}: Data Valuation using Deep Neural Networks at Initialization},
  author =       {Wu, Zhaoxuan and Shu, Yao and Low, Bryan Kian Hsiang},
  booktitle = 	 {Proceedings of the 39th International Conference on Machine Learning},
  pages = 	 {24150--24176},
  year = 	 {2022},
  editor = 	 {Chaudhuri, Kamalika and Jegelka, Stefanie and Song, Le and Szepesvari, Csaba and Niu, Gang and Sabato, Sivan},
  volume = 	 {162},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {17--23 Jul},
  publisher =    {PMLR},
  pdf = 	 {https://proceedings.mlr.press/v162/wu22j/wu22j.pdf},
  url = 	 {https://proceedings.mlr.press/v162/wu22j.html}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


### 2021

<details><summary><b>Validation Free and Replication Robust Volume-based Data Valuation</b> 
<br>
&emsp;<i>Xinyi Xu, Zhaoxuan Wu, Chuan Sheng Foo, Bryan Kian Hsiang Low</i>
<br>
&emsp;<i>Advances in Neural Information Processing Systems 34 (NeurIPS), 2021</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.neurips.cc/paper/2021/hash/59a3adea76fadcb6dd9e54c96fc155d1-Abstract.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/ZhaoxuanWu/VolumeBased-DataValuation">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Data valuation arises as a non-trivial challenge in real-world use cases such as collaborative machine learning, federated learning, trusted data sharing, data marketplaces. The value of data is often associated with the learning performance (e.g., validation accuracy) of a model trained on the data, which introduces a close coupling between data valuation and validation. However, a validation set may notbe available in practice and it can be challenging for the data providers to reach an agreement on the choice of the validation set. Another practical issue is that of data replication: Given the value of some data points, a dishonest data provider may replicate these data points to exploit the valuation for a larger reward/payment. We observe that the diversity of the data points is an inherent property of a dataset that is independent of validation. We formalize diversity via the volume of the data matrix (i.e., determinant of its left Gram), which allows us to establish a formal connection between the diversity of data and learning performance without requiring validation. Furthermore, we propose a robust volume measure with a theoretical guarantee on the replication robustness by following the intuition that copying the same data points does not increase the diversity of data. We perform extensive experiments to demonstrate its consistency in valuation and practical advantages over existing baselines and show that our method is model- and task-agnostic and can be flexibly adapted to handle various neural networks.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @inproceedings{Xu2021,
 author = {Xu, Xinyi and Wu, Zhaoxuan and Foo, Chuan Sheng and Low, Bryan Kian Hsiang},
 booktitle = {Advances in Neural Information Processing Systems},
 editor = {M. Ranzato and A. Beygelzimer and Y. Dauphin and P.S. Liang and J. Wortman Vaughan},
 pages = {10837--10848},
 publisher = {Curran Associates, Inc.},
 title = {Validation Free and Replication Robust Volume-based Data Valuation},
 volume = {34},
 year = {2021}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>

### 2020
<a id="2020-other"></a>

<details><summary><b>Data Valuation using Reinforcement Learning</b> 
<br>
&emsp;<i>Jinsung Yoon, Sercan Arik, Tomas Pfister</i>
<br>
&emsp;<i>Proceedings of the 37th International Conference on Machine Learning (ICML), 2020</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.mlr.press/v119/yoon20a.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/google-research/google-research/tree/master/dvrl">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Quantifying the value of data is a fundamental problem in machine learning and has multiple important use cases: (1) building insights about the dataset and task, (2) domain adaptation, (3) corrupted sample discovery, and (4) robust learning. We propose Data Valuation using Reinforcement Learning (DVRL), to adaptively learn data values jointly with the predictor model. DVRL uses a data value estimator (DVE) to learn how likely each datum is used in training of the predictor model. DVE is trained using a reinforcement signal that reflects performance on the target task. We demonstrate that DVRL yields superior data value estimates compared to alternative methods across numerous datasets and application scenarios. The corrupted sample discovery performance of DVRL is close to optimal in many regimes (i.e. as if the noisy samples were known apriori), and for domain adaptation and robust learning DVRL significantly outperforms state-of-the-art by 14.6% and 10.8%, respectively.
<br><br>

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @InProceedings{pmlr-v119-yoon20a,
  title = 	 {Data Valuation using Reinforcement Learning},
  author =       {Yoon, Jinsung and Arik, Sercan and Pfister, Tomas},
  booktitle = 	 {Proceedings of the 37th International Conference on Machine Learning},
  pages = 	 {10842--10851},
  year = 	 {2020},
  editor = 	 {III, Hal Daumé and Singh, Aarti},
  volume = 	 {119},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {13--18 Jul},
  publisher =    {PMLR},
  pdf = 	 {http://proceedings.mlr.press/v119/yoon20a/yoon20a.pdf},
  url = 	 {https://proceedings.mlr.press/v119/yoon20a.html}
}
</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


<details><summary><b>TITLE</b> 
<br>
&emsp;<i>AUTHORS</i>
<br>
&emsp;<i>VENUE</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> TEXT
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> BIBTEX
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>
