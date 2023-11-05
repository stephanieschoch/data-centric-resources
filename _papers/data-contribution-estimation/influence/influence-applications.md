---
layout: default
title: Influence Applications
parent: Influence Functions
grand_parent: Data Contribution Estimation
nav_order: 3
---

## Applications of Influence-based Data Contribution Estimation

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

### 2020

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
