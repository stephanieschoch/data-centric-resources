---
layout: default
title: Influence Applications
parent: Influence Functions
grand_parent: Data Contribution Estimation
nav_order: 3
---

## Applications of Influence-based Data Contribution Estimation

### 2023

<details><summary><b>Studying Large Language Model Generalization with Influence Functions</b> <br>
&emsp;<i>Roger Grosse, Juhan Bae, Cem Anil, Nelson Elhage, Alex Tamkin, Amirhossein Tajdini, Benoit Steiner, Dustin Li, Esin Durmus, Ethan Perez, Evan Hubinger, Kamilė Lukošiūtė, Karina Nguyen, Nicholas Joseph, Sam McCandlish, Jared Kaplan, Samuel R. Bowman</i><br>
&emsp;<i>arXiv, 2023</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2308.03296">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://www.anthropic.com/index/influence-functions">Blog</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> When trying to gain better visibility into a machine learning model in order to understand and mitigate the associated risks, a potentially valuable source of evidence is: which training examples most contribute to a given behavior? Influence functions aim to answer a counterfactual: how would the model's parameters (and hence its outputs) change if a given sequence were added to the training set? While influence functions have produced insights for small models, they are difficult to scale to large language models (LLMs) due to the difficulty of computing an inverse-Hessian-vector product (IHVP). We use the Eigenvalue-corrected Kronecker-Factored Approximate Curvature (EK-FAC) approximation to scale influence functions up to LLMs with up to 52 billion parameters. In our experiments, EK-FAC achieves similar accuracy to traditional influence function estimators despite the IHVP computation being orders of magnitude faster. We investigate two algorithmic techniques to reduce the cost of computing gradients of candidate training sequences: TF-IDF filtering and query batching. We use influence functions to investigate the generalization patterns of LLMs, including the sparsity of the influence patterns, increasing abstraction with scale, math and programming abilities, cross-lingual generalization, and role-playing behavior. Despite many apparently sophisticated forms of generalization, we identify a surprising limitation: influences decay to near-zero when the order of key phrases is flipped. Overall, influence functions give us a powerful new tool for studying the generalization properties of LLMs.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{grosse2023studying,
  title={Studying large language model generalization with influence functions},
  author={Grosse, Roger and Bae, Juhan and Anil, Cem and Elhage, Nelson and Tamkin, Alex and Tajdini, Amirhossein and Steiner, Benoit and Li, Dustin and Durmus, Esin and Perez, Ethan and others},
  journal={arXiv preprint arXiv:2308.03296},
  year={2023}
} </code></pre>
{% endraw %}
</details>

</blockquote></details>

### 2022
<details><summary><b>First is Better Than Last for Language Data Influence</b> <br>
&emsp;<i>Chih-Kuan Yeh, Ankur Taly, Mukund Sundararajan, Frederick Liu, Pradeep Kumar Ravikumar</i><br>
&emsp;<i>Advances in Neural Information Processing Systems (NeurIPS), 2022</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://openreview.net/forum?id=yfrDD_rmD5">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/chihkuanyeh/TracIn-WE">Code</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> The ability to identify influential training examples enables us to debug training data and explain model behavior. Existing techniques to do so are based on the flow of training data influence through the model parameters. For large models in NLP applications, it is often computationally infeasible to study this flow through all model parameters, therefore techniques usually pick the last layer of weights. However, we observe that since the activation connected to the last layer of weights contains "shared logic", the data influenced calculated via the last layer weights prone to a "cancellation effect", where the data influence of different examples have large magnitude that contradicts each other. The cancellation effect lowers the discriminative power of the influence score, and deleting influential examples according to this measure often does not change the model's behavior by much. To mitigate this, we propose a technique called TracIn-WE that modifies a method called TracIn to operate on the word embedding layer instead of the last layer, where the cancellation effect is less severe. One potential concern is that influence based on the word embedding layer may not encode sufficient high level information.  However, we find that gradients (unlike embeddings) do not suffer from this, possibly because they chain through higher layers. We show that TracIn-WE significantly outperforms other data influence methods applied on the last layer significantly on the case deletion evaluation on three language classification tasks for different models. In addition, TracIn-WE can produce scores not just at the level of the overall training input, but also at the level of words within the training input, a further aid in debugging. 
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @inproceedings{
yeh2022first,
title={First is Better Than Last for Language Data Influence},
author={Chih-Kuan Yeh and Ankur Taly and Mukund Sundararajan and Frederick Liu and Pradeep Kumar Ravikumar},
booktitle={Advances in Neural Information Processing Systems},
editor={Alice H. Oh and Alekh Agarwal and Danielle Belgrave and Kyunghyun Cho},
year={2022},
url={https://openreview.net/forum?id=yfrDD_rmD5}
} </code></pre>
{% endraw %}
</details>
</blockquote></details>


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
