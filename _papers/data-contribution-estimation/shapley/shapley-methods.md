---
layout: default
title: Shapley Methods
parent: Shapley Values
grand_parent: Data Contribution Estimation
nav_order: 2
---

## Shapley-based Methods for Data Contribution Estimation
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


<a id="2023-shapley"></a>

### 2022
<a id="2022-shapley"></a>

<details><summary><b>CS-Shapley: Class-wise Shapley Values for Data Valuation in Classification</b>
<br>
&emsp;<i>Stephanie Schoch, Haifeng Xu, Yangfeng Ji</i>
<br>
&emsp;<i>Advances in Neural Information Processing Systems 35 (NeurIPS), 2022</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://openreview.net/forum?id=KTOcrOR5mQ9">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/stephanieschoch/cs-shapley">Code</a>]
<br>
<br>
</summary>
<blockquote> <b>Abstract:</b> Data valuation, or the valuation of individual datum contributions, has seen growing interest in machine learning due to its demonstrable efficacy for tasks such as noisy label detection. In particular, due to the desirable axiomatic properties, several Shapley value approximation methods have been proposed. In these methods, the value function is typically defined as the predictive accuracy over the entire development set. However, this limits the ability to differentiate between training instances that are helpful or harmful to their own classes. Intuitively, instances that harm their own classes may be noisy or mislabeled and should receive a lower valuation than helpful instances. In this work, we propose CS-Shapley, a Shapley value with a new value function that discriminates between training instances' in-class and out-of-class contributions. Our theoretical analysis shows the proposed value function is (essentially) the unique function that satisfies two desirable properties for evaluating data values in classification. Further, our experiments on two benchmark evaluation tasks (data removal and noisy label detection) and four classifiers demonstrate the effectiveness of CS-Shapley over existing methods. Lastly, we evaluate the "transferability" of data values estimated from one classifier to others, and our results suggest Shapley-based data valuation is transferable for application across different models.
<br>
<br>
<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code>@inproceedings{
schoch2022csshapley,
title={{CS}-Shapley: Class-wise Shapley Values for Data Valuation in Classification},
author={Stephanie Schoch and Haifeng Xu and Yangfeng Ji}, 
booktitle={Advances in Neural Information Processing Systems},
editor={Alice H. Oh and Alekh Agarwal and Danielle Belgrave and Kyunghyun Cho},
year={2022},
url={https://openreview.net/forum?id=KTOcrOR5mQ9}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>

<details><summary><b>Beta Shapley: a Unified and Noise-reduced Data Valuation Framework for Machine Learning</b> 
<br>
&emsp;<i>Yongchan Kwon, James Zou</i>
<br>
&emsp;<i>Proceedings of The 25th International Conference on Artificial Intelligence and Statistics (AISTATS), 2022</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.mlr.press/v151/kwon22a.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/ykwon0407/beta_shapley">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Data Shapley has recently been proposed as a principled framework to quantify the contribution of individual datum in machine learning. It can effectively identify helpful or harmful data points for a learning algorithm. In this paper, we propose Beta Shapley, which is a substantial generalization of Data Shapley. Beta Shapley arises naturally by relaxing the efficiency axiom of the Shapley value, which is not critical for machine learning settings. Beta Shapley unifies several popular data valuation methods and includes data Shapley as a special case. Moreover, we prove that Beta Shapley has several desirable statistical properties and propose efficient algorithms to estimate it. We demonstrate that Beta Shapley outperforms state-of-the-art data valuation methods on several downstream ML tasks such as: 1) detecting mislabeled training data; 2) learning with subsamples; and 3) identifying points whose addition or removal have the largest positive or negative impact on the model.
<br>
<br>
<details><summary><b>Notes</b></summary>Generalization of Data Shapley that arises from relaxing the efficiency axiom. Parameterizes a Beta distribution to adjust the weights of different subset cardinalities for reduced noise (signal of marginal contribution of large cardinalities more susceptible to noise perturbation, so assign large weight to small cardinalities)
<br><br></details>

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @InProceedings{pmlr-v151-kwon22a,
  title = 	 { Beta Shapley: a Unified and Noise-reduced Data Valuation Framework for Machine Learning },
  author =       {Kwon, Yongchan and Zou, James},
  booktitle = 	 {Proceedings of The 25th International Conference on Artificial Intelligence and Statistics},
  pages = 	 {8780--8802},
  year = 	 {2022},
  editor = 	 {Camps-Valls, Gustau and Ruiz, Francisco J. R. and Valera, Isabel},
  volume = 	 {151},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {28--30 Mar},
  publisher =    {PMLR},
  pdf = 	 {https://proceedings.mlr.press/v151/kwon22a/kwon22a.pdf},
  url = 	 {https://proceedings.mlr.press/v151/kwon22a.html}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


<details><summary><b>Differentially Private Shapley Values for Data Evaluation</b>
<br>
&emsp;<i>Lauren Watson, Rayna Andreeva, Hao-Tsung Yang, Rik Sarkar</i>
<br>
&emsp;<i>arXiv, 2022</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2206.00511">Paper</a>]
<br>
<br>
</summary>
<blockquote> <b>Abstract:</b> The Shapley value has been proposed as a solution to many applications in machine learning, including for equitable valuation of data. Shapley values are computationally expensive and involve the entire dataset. The query for a point's Shapley value can also compromise the statistical privacy of other data points. We observe that in machine learning problems such as empirical risk minimization, and in many learning algorithms (such as those with uniform stability), a diminishing returns property holds, where marginal benefit per data point decreases rapidly with data sample size. Based on this property, we propose a new stratified approximation method called the Layered Shapley Algorithm. We prove that this method operates on small (O(\polylog(n))) random samples of data and small sized (O(log n)) coalitions to achieve the results with guaranteed probabilistic accuracy, and can be modified to incorporate differential privacy. Experimental results show that the algorithm correctly identifies high-value data points that improve validation accuracy, and that the differentially private evaluations preserve approximate ranking of data.
<br><br>

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{watson2022differentially,
  title={Differentially Private Shapley Values for Data Evaluation},
  author={Watson, Lauren and Andreeva, Rayna and Yang, Hao-Tsung and Sarkar, Rik},
  journal={arXiv preprint arXiv:2206.00511},
  year={2022}
}
</code></pre>
{% endraw %}
</details>
</blockquote>
</details>

### 2021
<a id="2021-shapley"></a>

<details><summary><b>Efficient Computation and Analysis of Distributional Shapley Values</b>
<br>
&emsp;<i>Yongchan Kwon, Manuel A. Rivas, James Zou</i>
<br>
&emsp;<i>Proceedings of The 24th International Conference on Artificial Intelligence and Statistics (AISTATS), 2021</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.mlr.press/v130/kwon21a.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/ykwon0407/fast_dist_shapley">Code</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://papertalk.org/papertalks/27757">Talk</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Distributional data Shapley value (DShapley) has recently been proposed as a principled framework to quantify the contribution of individual datum in machine learning. DShapley develops the foundational game theory concept of Shapley values into a statistical framework and can be applied to identify data points that are useful (or harmful) to a learning algorithm. Estimating DShapley is computationally expensive, however, and this can be a major challenge to using it in practice. Moreover, there has been little mathematical analyses of how this value depends on data characteristics. In this paper, we derive the first analytic expressions for DShapley for the canonical problems of linear regression, binary classification, and non-parametric density estimation. These analytic forms provide new algorithms to estimate DShapley that are several orders of magnitude faster than previous state-of-the-art methods. Furthermore, our formulas are directly interpretable and provide quantitative insights into how the value varies for different types of data. We demonstrate the practical efficacy of our approach on multiple real and synthetic datasets.
<br><br>
<details><summary><b>Bibtex</b></summary>    
{% raw %}
<pre><code> 
@InProceedings{pmlr-v130-kwon21a,
  title = 	 { Efficient Computation and Analysis of Distributional Shapley Values },
  author =       {Kwon, Yongchan and A. Rivas, Manuel and Zou, James},
  booktitle = 	 {Proceedings of The 24th International Conference on Artificial Intelligence and Statistics},
  pages = 	 {793--801},
  year = 	 {2021},
  editor = 	 {Banerjee, Arindam and Fukumizu, Kenji},
  volume = 	 {130},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {13--15 Apr},
  publisher =    {PMLR},
  pdf = 	 {http://proceedings.mlr.press/v130/kwon21a/kwon21a.pdf},
  url = 	 {https://proceedings.mlr.press/v130/kwon21a.html}
}
</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


<details><summary><b>Scalability vs. Utility: Do We Have to Sacrifice One for the Other in Data Importance Quantification?</b>
<br>
&emsp;<i>Ruoxi Jia, Fan Wu, Xuehui Sun, Jiacen Xu, David Dao, Bhavya Kailkhura, Ce Zhang, Bo Li, Dawn Song</i>
<br>
&emsp;<i>Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2021</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://openaccess.thecvf.com/content/CVPR2021/html/Jia_Scalability_vs._Utility_Do_We_Have_To_Sacrifice_One_for_CVPR_2021_paper.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/AI-secure/Shapley-Study">Code</a>]
<br>
<br>
</summary>
<blockquote> <b>Abstract:</b> Quantifying the importance of each training point to a learning task is a fundamental problem in machine learning and the estimated importance scores have been leveraged to guide a range of data workflows such as data summarization and domain adaption. One simple idea is to use the leave-one-out error of each training point to indicate its importance. Recent work has also proposed to use the Shapley value, as it defines a unique value distribution scheme that satisfies a set of appealing properties. However, calculating Shapley values is often expensive, which limits its applicability in real-world applications at scale. Multiple heuristics to improve the scalability of calculating Shapley values have been proposed recently, with the potential risk of compromising their utility in real-world applications. How well do existing data quantification methods perform on existing workflows? How do these methods compare with each other, empirically and theoretically? Must we sacrifice scalability for the utility in these workflows when using these methods? In this paper, we conduct a novel theoretical analysis comparing the utility of different importance quantification methods, and report extensive experimental studies on settings such as noisy label detection, watermark removal, data summarization, data acquisition, and domain adaptation on existing and proposed workflows. We show that Shapley value approximation based on a KNN surrogate over pre-trained feature embeddings obtains comparable utility with existing algorithms while achieving significant scalability improvement, often by orders of magnitude. Our theoretical analysis also justifies its advantage over the leave-one-out error. The code is available at https://github.com/AI-secure/Shapley-Study.
<br><br>
<details><summary><b>Notes</b></summary>KNN Surrogates
<br><br></details>
<details><summary><b>Bibtex</b></summary>    
{% raw %}
<pre><code> @InProceedings{Jia_2021_CVPR,
    author    = {Jia, Ruoxi and Wu, Fan and Sun, Xuehui and Xu, Jiacen and Dao, David and Kailkhura, Bhavya and Zhang, Ce and Li, Bo and Song, Dawn},
    title     = {Scalability vs. Utility: Do We Have To Sacrifice One for the Other in Data Importance Quantification?},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    month     = {June},
    year      = {2021},
    pages     = {8239-8247}
}
</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


<details><summary><b>Gradient Driven Rewards to Guarantee Fairness in Collaborative Machine Learning
</b> 
<br>
&emsp;<i>Xinyi Xu, Lingjuan Lyu, Xingjun Ma, Chenglin Miao, Chuan Sheng Foo, Bryan Kian Hsiang Low</i>
<br>
&emsp;<i>Advances in Neural Information Processing Systems 34 (NeurIPS), 2021</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.neurips.cc/paper/2021/hash/8682cc30db9c025ecd3fee433f8ab54c-Abstract.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/XinyiYS/Gradient-Driven-Rewards-to-Guarantee-Fairness-in-Collaborative-Machine-Learning">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> In collaborative machine learning(CML), multiple agents pool their resources(e.g., data) together for a common learning task. In realistic CML settings where the agents are self-interested and not altruistic, they may be unwilling to share data or model information without adequate rewards. Furthermore, as the data/model information shared by the agents may differ in quality, designing rewards which are fair to them is important so that they would not feel exploited nor discouraged from sharing. In this paper, we adopt federated learning as the CML paradigm, propose a novel cosine gradient Shapley value(CGSV) to fairly evaluate the expected marginal contribution of each agent’s uploaded model parameter update/gradient without needing an auxiliary validation dataset, and based on the CGSV, design a novel training-time gradient reward mechanism with a fairness guarantee by sparsifying the aggregated parameter update/gradient downloaded from the server as reward to each agent such that its resulting quality is commensurate to that of the agent’s uploaded parameter update/gradient. We empirically demonstrate the effectiveness of our fair gradient reward mechanism on multiple benchmark datasets in terms of fairness, predictive performance, and time overhead.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{xu2021gradient,
  title={Gradient driven rewards to guarantee fairness in collaborative machine learning},
  author={Xu, Xinyi and Lyu, Lingjuan and Ma, Xingjun and Miao, Chenglin and Foo, Chuan Sheng and Low, Bryan Kian Hsiang},
  journal={Advances in Neural Information Processing Systems},
  volume={34},
  pages={16104--16117},
  year={2021}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>

### 2020
<a id="2020-shapley"></a>

<details><summary><b>A Distributional Framework For Data Valuation</b>
<br>
&emsp;<i>Amirata Ghorbani, Michael Kim, James Zou</i>
<br>
&emsp;<i>Proceedings of the 37th International Conference on Machine Learning (ICML), 2020</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.mlr.press/v119/ghorbani20a.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/amiratag/DistributionalShapley">Code</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://papertalk.org/papertalks/6201">Talk</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Shapley value is a classic notion from game theory, historically used to quantify the contributions of individuals within groups, and more recently applied to assign values to data points when training machine learning models. Despite its foundational role, a key limitation of the data Shapley framework is that it only provides valuations for points within a fixed data set. It does not account for statistical aspects of the data and does not give a way to reason about points outside the data set. To address these limitations, we propose a novel framework – distributional Shapley– where the value of a point is defined in the context of an underlying data distribution. We prove that distributional Shapley has several desirable statistical properties; for example, the values are stable under perturbations to the data points themselves and to the underlying data distribution. We leverage these properties to develop a new algorithm for estimating values from data, which comes with formal guarantees and runs two orders of magnitude faster than state-of-the-art algorithms for computing the (non distributional) data Shapley values. We apply distributional Shapley to diverse data sets and demonstrate its utility in a data market setting.
<br><br>
<details><summary><b>Bibtex</b></summary>    
{% raw %}
<pre><code> 
@InProceedings{pmlr-v119-ghorbani20a,
  title = 	 {A Distributional Framework For Data Valuation},
  author =       {Ghorbani, Amirata and Kim, Michael and Zou, James},
  booktitle = 	 {Proceedings of the 37th International Conference on Machine Learning},
  pages = 	 {3535--3544},
  year = 	 {2020},
  editor = 	 {III, Hal Daumé and Singh, Aarti},
  volume = 	 {119},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {13--18 Jul},
  publisher =    {PMLR},
  pdf = 	 {http://proceedings.mlr.press/v119/ghorbani20a/ghorbani20a.pdf},
  url = 	 {https://proceedings.mlr.press/v119/ghorbani20a.html}
}
</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


### 2019
<a id="2019-shapley"></a>

<details><summary><b>Data Shapley: Equitable Valuation of Data for Machine Learning</b>
<br>
&emsp;<i>Amirata Ghorbani, James Zou</i>
<br>
&emsp;<i>Proceedings of the 36th International Conference on Machine Learning (ICML), 2019</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.mlr.press/v97/ghorbani19c.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/amiratag/DataShapley">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> As data becomes the fuel driving technological and economic growth, a fundamental challenge is how to quantify the value of data in algorithmic predictions and decisions. For example, in healthcare and consumer markets, it has been suggested that individuals should be compensated for the data that they generate, but it is not clear what is an equitable valuation for individual data. In this work, we develop a principled framework to address data valuation in the context of supervised machine learning. Given a learning algorithm trained on 𝑛 data points to produce a predictor, we propose data Shapley as a metric to quantify the value of each training datum to the predictor performance. Data Shapley uniquely satisfies several natural properties of equitable data valuation. We develop Monte Carlo and gradient-based methods to efficiently estimate data Shapley values in practical settings where complex learning algorithms, including neural networks, are trained on large datasets. In addition to being equitable, extensive experiments across biomedical, image and synthetic data demonstrate that data Shapley has several other benefits: 1) it is more powerful than the popular leave-one-out or leverage score in providing insight on what data is more valuable for a given learning task; 2) low Shapley value data effectively capture outliers and corruptions; 3) high Shapley value data inform what type of new data to acquire to improve the predictor.
<br><br>

<details><summary><b>Notes</b></summary>"Data Shapley" paper. Propose TMC-Shapley (truncated Monte Carlo Shapley) and G-Shapley (Gradient Shapley) approximations.
<br><br></details>

<details><summary><b>Bibtex</b></summary>   
{% raw %}
<pre><code> 
@InProceedings{pmlr-v97-ghorbani19c,
  title = 	 {Data Shapley: Equitable Valuation of Data for Machine Learning},
  author =       {Ghorbani, Amirata and Zou, James},
  booktitle = 	 {Proceedings of the 36th International Conference on Machine Learning},
  pages = 	 {2242--2251},
  year = 	 {2019},
  editor = 	 {Chaudhuri, Kamalika and Salakhutdinov, Ruslan},
  volume = 	 {97},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {09--15 Jun},
  publisher =    {PMLR},
  pdf = 	 {http://proceedings.mlr.press/v97/ghorbani19c/ghorbani19c.pdf},
  url = 	 {https://proceedings.mlr.press/v97/ghorbani19c.html}
}
</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


<details><summary><b>Towards Efficient Data Valuation Based on the Shapley Value</b>
<br>
&emsp;<i>Ruoxi Jia, David Dao, Boxin Wang, Frances Ann Hubis, Nick Hynes, Nezihe Merve Gürel, Bo Li, Ce Zhang, Dawn Song, Costas J. Spanos</i>
<br>
&emsp;<i>Proceedings of the Twenty-Second International Conference on Artificial Intelligence and Statistics (AISTATS), 2019</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.mlr.press/v89/jia19a.html">Paper</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> {\em “How much is my data worth?”} is an increasingly common question posed by organizations and individuals alike. An answer to this question could allow, for instance, fairly distributing profits among multiple data contributors and determining prospective compensation when data breaches happen. In this paper, we study the problem of \emph{data valuation} by utilizing the Shapley value, a popular notion of value which originated in coopoerative game theory. The Shapley value defines a unique payoff scheme that satisfies many desiderata for the notion of data value. However, the Shapley value often requires \emph{exponential} time to compute. To meet this challenge, we propose a repertoire of efficient algorithms for approximating the Shapley value. We also demonstrate the value of each training instance for various benchmark datasets.
<br><br>
<details><summary><b>Notes</b></summary>Shapley-based data valuation paper. Proposed various approximations including an influence function based heuristic.
<br><br></details>
<details><summary><b>Bibtex</b></summary>    
{% raw %}
<pre><code> 
@InProceedings{pmlr-v89-jia19a,
  title = 	 {Towards Efficient Data Valuation Based on the Shapley Value},
  author =       {Jia, Ruoxi and Dao, David and Wang, Boxin and Hubis, Frances Ann and Hynes, Nick and G\"{u}rel, Nezihe Merve and Li, Bo and Zhang, Ce and Song, Dawn and Spanos, Costas J.},
  booktitle = 	 {Proceedings of the Twenty-Second International Conference on Artificial Intelligence and Statistics},
  pages = 	 {1167--1176},
  year = 	 {2019},
  editor = 	 {Chaudhuri, Kamalika and Sugiyama, Masashi},
  volume = 	 {89},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {16--18 Apr},
  publisher =    {PMLR},
  pdf = 	 {http://proceedings.mlr.press/v89/jia19a/jia19a.pdf},
  url = 	 {https://proceedings.mlr.press/v89/jia19a.html}
}
</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


<details><summary><b>Efficient Task-Specific Data Valuation for Nearest Neighbor Algorithms</b> 
<br>
&emsp;<i>Ruoxi Jia, David Dao, Boxin Wang, Frances Ann Hubis, Nezihe Merve Gurel, Bo Li, Ce Zhang, Costas J. Spanos, Dawn Song</i>
<br>
&emsp;<i>Proceedings of the VLDB Endowment, 2019</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://vldb.org/pvldb/vol12/p1610-jia.pdf">Paper</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Given a data set  containing millions of data points and a data consumer who is willing to pay for $X to train a machine learning (ML) model over , how should we distribute this $X to each data point to reflect its "value"? In this paper, we define the "relative value of data" via the Shapley value, as it uniquely possesses properties with appealing real-world interpretations, such as fairness, rationality and decentralizability. For general, bounded utility functions, the Shapley value is known to be challenging to compute: to get Shapley values for all N data points, it requires O(2N) model evaluations for exact computation and O(NlogN) for (ϵ,δ)-approximation. In this paper, we focus on one popular family of ML models relying on K-nearest neighbors (KNN). The most surprising result is that for unweighted KNN classifiers and regressors, the Shapley value of all N data points can be computed, exactly, in O(NlogN) time -- an exponential improvement on computational complexity! Moreover, for (ϵ,δ)-approximation, we are able to develop an algorithm based on Locality Sensitive Hashing (LSH) with only sublinear complexity O(Nh(ϵ,K)logN) when ϵ is not too small and K is not too large. We empirically evaluate our algorithms on up to 10 million data points and even our exact algorithm is up to three orders of magnitude faster than the baseline approximation algorithm. The LSH-based approximation algorithm can accelerate the value calculation process even further. We then extend our algorithms to other scenarios such as (1) weighed KNN classifiers, (2) different data points are clustered by different data curators, and (3) there are data analysts providing computation who also requires proper valuation.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{jia12efficient,
  title={Efficient Task-Specific Data Valuation for Nearest Neighbor Algorithms},
  author={Jia, Ruoxi and Dao, David and Wang, Boxin and Hubis, Frances Ann and Gurel, Nezihe Merve and Zhang, Bo Li4 Ce and Song, Costas Spanos1 Dawn},
  journal={Proceedings of the VLDB Endowment},
  volume={12},
  number={11}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>