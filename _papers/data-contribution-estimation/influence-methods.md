---
layout: page
title: Influence Methods
parent: Data Contribution Estimation
nav_order: 2
---

## Influence-Methods
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
<details><summary><b>Resolving Training Biases via Influence-based Data Relabeling</b> 
<br>
&emsp;<i>Shuming Kong, Yanyan Shen, Linpeng Huang</i>
<br>
&emsp;<i>International Conference on Learning Representations (ICLR), 2022</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://openreview.net/forum?id=EskfH0bwNVn">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/Viperccc/RDIA">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> The performance of supervised learning methods easily suffers from the training bias issue caused by train-test distribution mismatch or label noise. Influence function is a  technique that estimates the impacts of a training sample on the model’s predictions. Recent studies on \emph{data resampling} have employed influence functions to identify \emph{harmful} training samples that will degrade model's test performance. They have shown that discarding or downweighting the identified harmful training samples is an effective way to resolve training biases. In this work, we move one step forward and propose an influence-based relabeling framework named RDIA for reusing harmful training samples toward better model performance. To achieve this, we use influence functions to estimate how relabeling a training sample would affect model's test performance and further develop a novel relabeling function R. We theoretically prove that applying R to relabel harmful training samples allows the model to achieve lower test loss than simply discarding them for any classification tasks using cross-entropy loss. Extensive experiments on ten real-world datasets demonstrate RDIA outperforms the state-of-the-art data resampling methods and improves model's robustness against label noise.
<br><br>

<details><summary><b>Notes</b></summary>Rather than discarding harmful examples, uses influence functions to estimate how relabeling a training sample would affect a model’s test performance (and also develops a new relabeling function). Improves model robustness to label noise and achieves lower test loss than just discarding the harmful examples.
<br><br></details>

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @inproceedings{
kong2022resolving,
title={Resolving Training Biases via Influence-based Data Relabeling},
author={Shuming Kong and Yanyan Shen and Linpeng Huang},
booktitle={International Conference on Learning Representations},
year={2022},
url={https://openreview.net/forum?id=EskfH0bwNVn}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


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


<details><summary><b>Explaining Black Box Predictions and Unveiling Data Artifacts through Influence Functions</b>
<br>
&emsp;<i>Xiaochuang Han, Byron C. Wallace, Yulia Tsvetkov</i>
<br>
&emsp;<i>Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics (ACL), 2020</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://aclanthology.org/2020.acl-main.492/">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/xhan77/influence-function-analysis">Code</a>]
<br><br></summary>
  
<blockquote> <b>Abstract:</b> Modern deep learning models for NLP are notoriously opaque. This has motivated the development of methods for interpreting such models, e.g., via gradient-based saliency maps or the visualization of attention weights. Such approaches aim to provide explanations for a particular model prediction by highlighting important words in the corresponding input text. While this might be useful for tasks where decisions are explicitly influenced by individual tokens in the input, we suspect that such highlighting is not suitable for tasks where model decisions should be driven by more complex reasoning. In this work, we investigate the use of influence functions for NLP, providing an alternative approach to interpreting neural text classifiers. Influence functions explain the decisions of a model by identifying influential training examples. Despite the promise of this approach, influence functions have not yet been extensively evaluated in the context of NLP, a gap addressed by this work. We conduct a comparison between influence functions and common word-saliency methods on representative tasks. As suspected, we find that influence functions are particularly useful for natural language inference, a task in which ‘saliency maps’ may not have clear interpretation. Furthermore, we develop a new quantitative measure based on influence functions that can reveal artifacts in training data.
<br><br> 

<details><summary><b>Bibtex</b></summary>   
{% raw %}
<pre><code> @inproceedings{han-etal-2020-explaining,
    title = "Explaining Black Box Predictions and Unveiling Data Artifacts through Influence Functions",
    author = "Han, Xiaochuang  and
      Wallace, Byron C.  and
      Tsvetkov, Yulia",
    editor = "Jurafsky, Dan  and
      Chai, Joyce  and
      Schluter, Natalie  and
      Tetreault, Joel",
    booktitle = "Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics",
    month = jul,
    year = "2020",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2020.acl-main.492",
    doi = "10.18653/v1/2020.acl-main.492",
    pages = "5553--5563"
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


<details><summary><b>Less Is Better: Unweighted Data Subsampling via Influence Function</b> 
<br>
&emsp;<i>Zifeng Wang, Hong Zhu, Zhenhua Dong, Xiuqiang He, Shao-Lun Huang</i>
<br>
&emsp;<i>Proceedings of the AAAI Conference on Artificial Intelligence (AAAI), 2020</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/1912.01321">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/RyanWangZf/Influence_Subsampling">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> In the time of Big Data, training complex models on large-scale data sets is challenging, making it appealing to reduce data volume for saving computation resources by subsampling. Most previous works in subsampling are weighted methods designed to help the performance of subset-model approach the full-set-model, hence the weighted methods have no chance to acquire a subset-model that is better than the full-set-model. However, we question that how can we achieve better model with less data? In this work, we propose a novel Unweighted Influence Data Subsampling (UIDS) method, and prove that the subset-model acquired through our method can outperform the full-set-model. Besides, we show that overly confident on a given test set for sampling is common in Influence-based subsampling methods, which can eventually cause our subset-model's failure in out-of-sample test. To mitigate it, we develop a probabilistic sampling scheme to control the worst-case risk over all distributions close to the empirical distribution. The experiment results demonstrate our methods superiority over existed subsampling methods in diverse tasks, such as text classification, image classification, click-through prediction, etc.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @inproceedings{wang2019less,
  title={Less Is Better: Unweighted Data Subsampling via Influence Function},
  author={Wang, Zifeng and Zhu, Hong and Dong, Zhenhua and He, Xiuqiang and Huang, Shao-Lun},
  booktitle={Proceedings of the AAAI Conference on Artificial Intelligence (AAAI)},
  year={2020}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>

### 2018
<details><summary><b>Optimal Subsampling with Influence Functions</b> 
<br>
&emsp;<i>Daniel Ting, Eric Brochu</i>
<br>
&emsp;<i>Advances in Neural Information Processing Systems (NeurIPS), 2018</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://papers.nips.cc/paper/2018/hash/57c0531e13f40b91b3b0f1a30b529a1d-Abstract.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="">Code</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> Subsampling is a common and often effective method to deal with the computational challenges of large datasets. However, for most statistical models, there is no well-motivated approach for drawing a non-uniform subsample. We show that the concept of an asymptotically linear estimator and the associated influence function leads to asymptotically optimal sampling probabilities for a wide class of popular models. This is the only tight optimality result for subsampling we are aware of as other methods only provide probabilistic error bounds or optimal rates. Furthermore, for linear regression models, which have well-studied procedures for non-uniform subsampling, we empirically show our optimal influence function based method outperforms previous approaches even when using approximations to the optimal probabilities.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{ting2018optimal,
  title={Optimal subsampling with influence functions},
  author={Ting, Daniel and Brochu, Eric},
  journal={Advances in neural information processing systems},
  volume={31},
  year={2018}
}
</code></pre>
{% endraw %}
</details>
</blockquote>
</details>


### 2017
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
