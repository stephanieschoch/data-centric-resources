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

### 2023

<details><summary><b>LAVA: Data Valuation without Pre-Specified Learning Algorithms</b> <br>
&emsp;<i>Hoang Anh Just, Feiyang Kang, Jiachen T. Wang, Yi Zeng, Myeongseob Ko, Ming Jin, Ruoxi Jia</i><br>
&emsp;<i>The Eleventh International Conference on Learning Representations (ICLR), 2023</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://openreview.net/forum?id=JJuP86nBl4q">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/ruoxi-jia-group/LAVA">Code</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> Traditionally, data valuation is posed as a problem of equitably splitting the validation performance of a learning algorithm among the training data. As a result, the calculated data values depend on many design choices of the underlying learning algorithm. However, this dependence is undesirable for many use cases of data valuation, such as setting priorities over different data sources in a data acquisition process and informing pricing mechanisms in a data marketplace. In these scenarios, data needs to be valued before the actual analysis and the choice of the learning algorithm is still undetermined then. Another side-effect of the dependence is that to assess the value of individual points, one needs to re-run the learning algorithm with and without a point, which incurs a large computation burden. This work leapfrogs over the current limits of data valuation methods by introducing a new framework that can value training data in a way that is oblivious to the downstream learning algorithm. (1) We develop a proxy for the validation performance associated with a training set based on a non-conventional class-wise Wasserstein distance between the training and the validation set. We show that the distance characterizes the upper bound of the validation performance for any given model under certain Lipschitz conditions. (2) We develop a novel method to value individual data based on the sensitivity analysis of the class-wise Wasserstein distance. Importantly, these values can be directly obtained for free from the output of off-the-shelf optimization solvers when computing the distance. (3) We evaluate our new data valuation framework over various use cases related to detecting low-quality data and show that, surprisingly, the learning-agnostic feature of our framework enables a significant improvement over the state-of-the-art performance while being orders of magnitude faster.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @inproceedings{
just2023lava,
title={{LAVA}: Data Valuation without Pre-Specified Learning Algorithms},
author={Hoang Anh Just and Feiyang Kang and Tianhao Wang and Yi Zeng and Myeongseob Ko and Ming Jin and Ruoxi Jia},
booktitle={The Eleventh International Conference on Learning Representations },
year={2023},
url={https://openreview.net/forum?id=JJuP86nBl4q}
} </code></pre>
{% endraw %}
</details>

</blockquote></details>


<details><summary><b>Data Banzhaf: A Robust Data Valuation Framework for Machine Learning</b> <br>
&emsp;<i>Jiachen T. Wang, Ruoxi Jia</i><br>
&emsp;<i>Proceedings of The 26th International Conference on Artificial Intelligence and Statistics (AISTATS), 2023</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.mlr.press/v206/wang23e">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/Jiachen-T-Wang/data-banzhaf">Code</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> Data valuation has wide use cases in machine learning, including improving data quality and creating economic incentives for data sharing. This paper studies the robustness of data valuation to noisy model performance scores. Particularly, we find that the inherent randomness of the widely used stochastic gradient descent can cause existing data value notions (e.g., the Shapley value and the Leave-one-out error) to produce inconsistent data value rankings across different runs. To address this challenge, we introduce the concept of safety margin, which measures the robustness of a data value notion. We show that the Banzhaf value, a famous value notion that originated from cooperative game theory literature, achieves the largest safety margin among all semivalues (a class of value notions that satisfy crucial properties entailed by ML applications and include the famous Shapley value and Leave-one-out error). We propose an algorithm to efficiently estimate the Banzhaf value based on the Maximum Sample Reuse (MSR) principle. Our evaluation demonstrates that the Banzhaf value outperforms the existing semivalue-based data value notions on several ML tasks such as learning with weighted samples and noisy label detection. Overall, our study suggests that when the underlying ML algorithm is stochastic, the Banzhaf value is a promising alternative to the other semivalue-based data value schemes given its computational advantage and ability to robustly differentiate data quality.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> 
@InProceedings{pmlr-v206-wang23e,
  title = 	 {Data Banzhaf: A Robust Data Valuation Framework for Machine Learning},
  author =       {Wang, Jiachen T. and Jia, Ruoxi},
  booktitle = 	 {Proceedings of The 26th International Conference on Artificial Intelligence and Statistics},
  pages = 	 {6388--6421},
  year = 	 {2023},
  editor = 	 {Ruiz, Francisco and Dy, Jennifer and van de Meent, Jan-Willem},
  volume = 	 {206},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {25--27 Apr},
  publisher =    {PMLR},
  pdf = 	 {https://proceedings.mlr.press/v206/wang23e/wang23e.pdf},
  url = 	 {https://proceedings.mlr.press/v206/wang23e.html},
  abstract = 	 {Data valuation has wide use cases in machine learning, including improving data quality and creating economic incentives for data sharing. This paper studies the robustness of data valuation to noisy model performance scores. Particularly, we find that the inherent randomness of the widely used stochastic gradient descent can cause existing data value notions (e.g., the Shapley value and the Leave-one-out error) to produce inconsistent data value rankings across different runs. To address this challenge, we introduce the concept of safety margin, which measures the robustness of a data value notion. We show that the Banzhaf value, a famous value notion that originated from cooperative game theory literature, achieves the largest safety margin among all semivalues (a class of value notions that satisfy crucial properties entailed by ML applications and include the famous Shapley value and Leave-one-out error). We propose an algorithm to efficiently estimate the Banzhaf value based on the Maximum Sample Reuse (MSR) principle. Our evaluation demonstrates that the Banzhaf value outperforms the existing semivalue-based data value notions on several ML tasks such as learning with weighted samples and noisy label detection. Overall, our study suggests that when the underlying ML algorithm is stochastic, the Banzhaf value is a promising alternative to the other semivalue-based data value schemes given its computational advantage and ability to robustly differentiate data quality.}
} </code></pre>
{% endraw %}
</details>

</blockquote></details>


<details><summary><b>Data-OOB: Out-of-bag Estimate as a Simple and Efficient Data Value</b> <br>
&emsp;<i>Yongchan Kwon, James Zou</i><br>
&emsp;<i>Proceedings of the 40th International Conference on Machine Learning (ICML), 2023</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2304.07718">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/ykwon0407/dataoob">Code</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> Data valuation is a powerful framework for providing statistical insights into which data are beneficial or detrimental to model training. Many Shapley-based data valuation methods have shown promising results in various downstream tasks, however, they are well known to be computationally challenging as it requires training a large number of models. As a result, it has been recognized as infeasible to apply to large datasets. To address this issue, we propose Data-OOB, a new data valuation method for a bagging model that utilizes the out-of-bag estimate. The proposed method is computationally efficient and can scale to millions of data by reusing trained weak learners. Specifically, Data-OOB takes less than 2.25 hours on a single CPU processor when there are 106 samples to evaluate and the input dimension is 100. Furthermore, Data-OOB has solid theoretical interpretations in that it identifies the same important data point as the infinitesimal jackknife influence function when two different points are compared. We conduct comprehensive experiments using 12 classification datasets, each with thousands of sample sizes. We demonstrate that the proposed method significantly outperforms existing state-of-the-art data valuation methods in identifying mislabeled data and finding a set of helpful (or harmful) data points, highlighting the potential for applying data values in real-world applications.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{kwon2023data,
  title={Data-OOB: Out-of-bag Estimate as a Simple and Efficient Data Value},
  author={Kwon, Yongchan and Zou, James},
  journal={Proceedings of the 40th International Conference on Machine Learning},
  year={2023}
} </code></pre>
{% endraw %}
</details>

</blockquote></details>


<details><summary><b>Data Valuation Without Training of a Model</b> <br>
&emsp;<i>Ki Nohyun, Hoyong Choi, Hye Won Chung</i><br>
&emsp;<i>The Eleventh International Conference on Learning Representations (ICLR), 2023 </i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://openreview.net/forum?id=XIzO8zr-WbM">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/JJchy/CG_score">Code</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> Many recent works on understanding deep learning try to quantify how much individual data instances influence the optimization and generalization of a model. Such attempts reveal characteristics and importance of individual instances, which may provide useful information in diagnosing and improving deep learning. However, most of the existing works on data valuation require actual training of a model, which often demands high-computational cost. In this paper, we provide a training-free data valuation score, called complexity-gap score, which is a data-centric score to quantify the influence of individual instances in generalization of two-layer overparameterized neural networks. The proposed score can quantify irregularity of the instances and measure how much each data instance contributes in the total movement of the network parameters during training. We theoretically analyze and empirically demonstrate the effectiveness of the complexity-gap score in finding `irregular or mislabeled' data instances, and also provide applications of the score in analyzing datasets and diagnosing training dynamics. Our code is publicly available at https://github.com/JJchy/CG_score.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @inproceedings{
nohyun2023data,
title={Data Valuation Without Training of a Model},
author={Ki Nohyun and Hoyong Choi and Hye Won Chung},
booktitle={The Eleventh International Conference on Learning Representations },
year={2023},
url={https://openreview.net/forum?id=XIzO8zr-WbM}
} </code></pre>
{% endraw %}
</details>

</blockquote></details>

### 2022

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

<details><summary><b>If You Like Shapley Then You'll Love the Core</b> <br>
&emsp;<i>Tom Yan, Ariel D. Procaccia</i><br>
&emsp;<i>Proceedings of the AAAI Conference on Artificial Intelligence (AAAI), 2021</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://cdn.aaai.org/ojs/16721/16721-13-20215-1-2-20210518.pdf">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="">Code</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> The prevalent approach to problems of credit assignment in machine learning — such as feature and data valuation— is to model the problem at hand as a cooperative game and apply the Shapley value. But cooperative game theory offers a rich menu of alternative solution concepts, which famously includes the core and its variants. Our goal is to challenge the machine learning community’s current consensus around the Shapley value, and make a case for the core as a viable alternative. To that end, we prove that arbitrarily good approximations to the least core — a core relaxation that is always feasible — can be computed efficiently (but prove an impossibility for a more refined solution concept, the nucleolus). We also perform experiments that corroborate these theoretical results and shed light on settings where the least core maybe preferable to the Shapley value.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @inproceedings{yan2021if,
  title={If you like shapley then you’ll love the core},
  author={Yan, Tom and Procaccia, Ariel D},
  booktitle={Proceedings of the AAAI Conference on Artificial Intelligence},
  volume={35},
  number={6},
  pages={5751--5759},
  year={2021}
} </code></pre>
{% endraw %}
</details>

</blockquote></details>


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


