---
layout: default
title: Influence Methods
parent: Influence Functions
grand_parent: Data Contribution Estimation
nav_order: 2
---

## Influence-based Methods for Data Contribution Estimation
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


### 2022


### 2021
<details><summary><b>FastIF: Scalable Influence Functions for Efficient Model Interpretation and Debugging</b> 
<br>
&emsp;<i>Han Guo, Nazneen Rajani, Peter Hase, Mohit Bansal, Caiming Xiong</i>
<br>
&emsp;<i>Proceedings of the 2021 Conference on Empirical Methods in Natural Language Processing (EMNLP), 2021</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://aclanthology.org/2021.emnlp-main.808/">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/salesforce/fast-influence-functions">Code</a>]
[<a target="_blank" rel="nonopener noreferrer" href="https://aclanthology.org/2021.emnlp-main.808.mp4">Talk</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Influence functions approximate the “influences” of training data-points for test predictions and have a wide variety of applications. Despite the popularity, their computational cost does not scale well with model and training data size. We present FastIF, a set of simple modifications to influence functions that significantly improves their run-time. We use k-Nearest Neighbors (kNN) to narrow the search space down to a subset of good candidate data points, identify the configurations that best balance the speed-quality trade-off in estimating the inverse Hessian-vector product, and introduce a fast parallel variant. Our proposed method achieves about 80X speedup while being highly correlated with the original influence values. With the availability of the fast influence functions, we demonstrate their usefulness in four applications. First, we examine whether influential data-points can “explain” test time behavior using the framework of simulatability. Second, we visualize the influence interactions between training and test data-points. Third, we show that we can correct model errors by additional fine-tuning on certain influential data-points, improving the accuracy of a trained MultiNLI model by 2.5% on the HANS dataset. Finally, we experiment with a similar setup but fine-tuning on datapoints not seen during training, improving the model accuracy by 2.8% and 1.7% on HANS and ANLI datasets respectively. Overall, our fast influence functions can be efficiently applied to large models and datasets, and our experiments demonstrate the potential of influence functions in model interpretation and correcting model errors.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code>@inproceedings{guo-etal-2021-fastif,
    title = "{F}ast{IF}: Scalable Influence Functions for Efficient Model Interpretation and Debugging",
    author = "Guo, Han  and
      Rajani, Nazneen  and
      Hase, Peter  and
      Bansal, Mohit  and
      Xiong, Caiming",
    editor = "Moens, Marie-Francine  and
      Huang, Xuanjing  and
      Specia, Lucia  and
      Yih, Scott Wen-tau",
    booktitle = "Proceedings of the 2021 Conference on Empirical Methods in Natural Language Processing",
    month = nov,
    year = "2021",
    address = "Online and Punta Cana, Dominican Republic",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2021.emnlp-main.808",
    doi = "10.18653/v1/2021.emnlp-main.808",
    pages = "10333--10350"
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


<details><summary><b>Influence Functions in Deep Learning Are Fragile </b> 
<br>
&emsp;<i>Samyadeep Basu, Phil Pope, Soheil Feizi</i>
<br>
&emsp;<i>International Conference on Learning Representations (ICLR), 2021</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://openreview.net/forum?id=xHKVVHGDOEk">Paper</a>]
<!--
[<a target="_blank" rel="noopener noreferrer" href="">Code</a>]
-->
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Influence functions approximate the effect of training samples in test-time predictions and have a wide variety of applications in machine learning interpretability and uncertainty estimation. A commonly-used (first-order) influence function can be implemented efficiently as a post-hoc method requiring access only to the gradients and Hessian of the model. For linear models, influence functions are well-defined due to the convexity of the underlying loss function and are generally accurate even across difficult settings where model changes are fairly large such as estimating group influences. Influence functions, however, are not well-understood in the context of deep learning with non-convex loss functions.  In this paper, we provide a comprehensive and large-scale empirical study of successes and failures of influence functions in neural network models trained on datasets such as Iris, MNIST, CIFAR-10 and ImageNet. Through our extensive experiments, we show that the network architecture, its depth and width, as well as the extent of model parameterization and regularization techniques have strong effects in the accuracy of influence functions. In particular, we find that (i) influence estimates are fairly accurate for shallow networks, while for deeper networks the estimates are often erroneous; (ii) for certain network architectures and datasets, training with weight-decay regularization is important to get high-quality influence estimates; and (iii) the accuracy of influence estimates can vary significantly depending on the examined test points. These results suggest that in general influence functions in deep learning are fragile and call for developing improved influence estimation methods to mitigate these issues in non-convex setups.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code>@inproceedings{
basu2021influence,
title={Influence Functions in Deep Learning Are Fragile},
author={Samyadeep Basu and Phil Pope and Soheil Feizi},
booktitle={International Conference on Learning Representations},
year={2021},
url={https://openreview.net/forum?id=xHKVVHGDOEk}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


### 2020
<a id="2020-influence"></a>
<details><summary><b>Estimating Training Data Influence by Tracing Gradient Descent</b> 
<br>
&emsp;<i>Garima Pruthi, Frederick Liu, Satyen Kale, Mukund Sundararajan</i>
<br>
&emsp;<i>Advances in Neural Information Processing Systems (NeurIPS), 2020</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.neurips.cc/paper/2020/hash/e6385d39ec9394f2f3a354d9d2b88eec-Abstract.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/frederick0329/TracIn">Code</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://videos.neurips.cc/category/34/search/Estimating%20Training%20Data/video/slideslive-38936700?t=27">Overview Talk</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://videos.neurips.cc/category/34/search/Estimating%20Training%20Data/video/slideslive-38937872?t=0">Spotlight Talk</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/frederick0329/TracIn/blob/master/figures/neurips_poster.pdf">Poster</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> We introduce a method called TracIn that computes the influence of a training example on a prediction made by the model. The idea is to trace how the loss on the test point changes during the training process whenever the training example of interest was utilized. We provide a scalable implementation of TracIn via: (a) a first-order gradient approximation to the exact computation, (b) saved checkpoints of standard training procedures, and (c) cherry-picking layers of a deep neural network. In contrast with previously proposed methods, TracIn is simple to implement; all it needs is the ability to work with gradients, checkpoints, and loss functions. The method is general. It applies to any machine learning model trained using stochastic gradient descent or a variant of it, agnostic of architecture, domain and task. We expect the method to be widely useful within processes that study and improve training data.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{pruthi2020estimating,
  title={Estimating training data influence by tracing gradient descent},
  author={Pruthi, Garima and Liu, Frederick and Kale, Satyen and Sundararajan, Mukund},
  journal={Advances in Neural Information Processing Systems},
  volume={33},
  pages={19920--19930},
  year={2020}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


<details><summary><b>On Second-Order Group Influence Functions for Black-Box Predictions</b>
<br>
&emsp;<i>Samyadeep Basu, Xuchen You, Soheil Feizi</i>
<br>
&emsp;<i>Proceedings of the 37th International Conference on Machine Learning (ICML), 2020</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.mlr.press/v119/basu20b.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="LINK">Code</a>]
<br><br></summary>
  
<blockquote> <b>Abstract:</b> With the rapid adoption of machine learning systems in sensitive applications, there is an increasing need to make black-box models explainable. Often we want to identify an influential group of training samples in a particular test prediction for a given machine learning model. Existing influence functions tackle this problem by using first-order approximations of the effect of removing a sample from the training set on model parameters. To compute the influence of a group of training samples (rather than an individual point) in model predictions, the change in optimal model parameters after removing that group from the training set can be large. Thus, in such cases, the first-order approximation can be loose. In this paper, we address this issue and propose second-order influence functions for identifying influential groups in test-time predictions. For linear models, across different sizes and types of groups, we show that using the proposed second-order influence function improves the correlation between the computed influence values and the ground truth ones. We also show that second-order influence functions could be used with optimization techniques to improve the selection of the most influential group for a test-sample.
<br><br>

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @InProceedings{pmlr-v119-basu20b,
  title = 	 {On Second-Order Group Influence Functions for Black-Box Predictions},
  author =       {Basu, Samyadeep and You, Xuchen and Feizi, Soheil},
  booktitle = 	 {Proceedings of the 37th International Conference on Machine Learning},
  pages = 	 {715--724},
  year = 	 {2020},
  editor = 	 {III, Hal Daumé and Singh, Aarti},
  volume = 	 {119},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {13--18 Jul},
  publisher =    {PMLR},
  pdf = 	 {http://proceedings.mlr.press/v119/basu20b/basu20b.pdf},
  url = 	 {https://proceedings.mlr.press/v119/basu20b.html}
}
</code></pre>
{% endraw %}
</details>

</blockquote></details>


<details><summary><b>Multi-Stage Influence Function</b> 
<br>
&emsp;<i>Hongge Chen, Si Si, Yang Li, Ciprian Chelba, Sanjiv Kumar, Duane Boning, Cho-Jui Hsieh</i>
<br>
&emsp;<i>Advances in Neural Information Processing Systems 33 (NeurIPS), 2020</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.neurips.cc/paper/2020/hash/95e62984b87e90645a5cf77037395959-Abstract.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Multi-stage training and knowledge transfer, from a large-scale pretraining task to various finetuning tasks, have revolutionized natural language processing and computer vision resulting in state-of-the-art performance improvements. In this paper, we develop a multi-stage influence function score to track predictions from a finetuned model all the way back to the pretraining data. With this score, we can identify the pretraining examples in the pretraining task that contribute most to a prediction in the finetuning task. The proposed multi-stage influence function generalizes the original influence function for a single model in (Koh &Liang, 2017), thereby enabling influence computation through both pretrained and finetuned models. We study two different scenarios with the pretrained embedding fixed or updated in the finetuning tasks. We test our proposed method in various experiments to show its effectiveness and potential applications.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{chen2020multi,
  title={Multi-stage influence function},
  author={Chen, Hongge and Si, Si and Li, Yang and Chelba, Ciprian and Kumar, Sanjiv and Boning, Duane and Hsieh, Cho-Jui},
  journal={Advances in Neural Information Processing Systems},
  volume={33},
  pages={12732--12742},
  year={2020}
}
</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


### 2019

<details><summary><b>On the Accuracy of Influence Functions for Measuring Group Effects</b> 
<br>
&emsp;<i>Pang Wei Koh, Kai-Siang Ang, Hubert H. K. Teo, Percy Liang</i>
<br>
&emsp;<i>Advances in Neural Information Processing Systems (NeurIPS), 2019</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://openreview.net/forum?id=HJentVSgUB">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/kohpangwei/group-influence-release">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Influence functions estimate the effect of removing a training point on a model without the need to retrain. They are based on a first-order Taylor approximation that is guaranteed to be accurate for sufficiently small changes to the model, and so are commonly used to study the effect of individual points in large datasets. However, we often want to study the effects of large groups of training points, e.g., to diagnose batch effects or apportion credit between different data sources. Removing such large groups can result in significant changes to the model. Are influence functions still accurate in this setting? In this paper, we find that across many different types of groups and for a range of real-world datasets, the predicted effect (using influence functions) of a group correlates surprisingly well with its actual effect, even if the absolute and relative errors are large. Our theoretical analysis shows that such strong correlation arises only under certain settings and need not hold in general, indicating that real-world datasets have particular properties that allow the influence approximation to be accurate.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{koh2019accuracy,
  title={On the accuracy of influence functions for measuring group effects},
  author={Koh, Pang Wei W and Ang, Kai-Siang and Teo, Hubert and Liang, Percy S},
  journal={Advances in neural information processing systems},
  volume={32},
  year={2019}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>



### 2018


### 2017
<details><summary><b>Understanding Black-box Predictions via Influence Functions</b> 
<br>
&emsp;<i>Pang Wei Koh, Percy Liang</i>
<br>
&emsp;<i>Proceedings of the 34th International Conference on Machine Learning (ICML), 2017</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.mlr.press/v70/koh17a">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/kohpangwei/influence-release">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> How can we explain the predictions of a black-box model? In this paper, we use influence functions — a classic technique from robust statistics — to trace a model’s prediction through the learning algorithm and back to its training data, thereby identifying training points most responsible for a given prediction. To scale up influence functions to modern machine learning settings, we develop a simple, efficient implementation that requires only oracle access to gradients and Hessian-vector products. We show that even on non-convex and non-differentiable models where the theory breaks down, approximations to influence functions can still provide valuable information. On linear models and convolutional neural networks, we demonstrate that influence functions are useful for multiple purposes: understanding model behavior, debugging models, detecting dataset errors, and even creating visually-indistinguishable training-set attacks.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> 
@InProceedings{pmlr-v70-koh17a,
  title = 	 {Understanding Black-box Predictions via Influence Functions},
  author =       {Pang Wei Koh and Percy Liang},
  booktitle = 	 {Proceedings of the 34th International Conference on Machine Learning},
  pages = 	 {1885--1894},
  year = 	 {2017},
  editor = 	 {Precup, Doina and Teh, Yee Whye},
  volume = 	 {70},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {06--11 Aug},
  publisher =    {PMLR},
  pdf = 	 {http://proceedings.mlr.press/v70/koh17a/koh17a.pdf},
  url = 	 {https://proceedings.mlr.press/v70/koh17a.html}}
</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


