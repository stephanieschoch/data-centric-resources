---
layout: default
title: Currently Uncategorized
nav_order: 3
has_children: false
has_toc: false
---

# Currently Uncategorized
Contains papers that will be moved to other sections as the repository continues to be developed.

## Papers
<details><summary><b>Coresets for Data-efficient Training of Machine Learning Models</b>
<br>
&emsp;<i>Baharan Mirzasoleiman, Jeff Bilmes, Jure Leskovec</i>
<br>
&emsp;<i>Proceedings of the 37th International Conference on Machine Learning (ICML), 2020</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://proceedings.mlr.press/v119/mirzasoleiman20a.html">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/baharanm/craig">Code</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://icml.cc/media/icml-2020/Slides/6325.pdf">Slides</a>]
<br><br></summary>
  
<blockquote> <b>Abstract:</b> Incremental gradient (IG) methods, such as stochastic gradient descent and its variants are commonly used for large scale optimization in machine learning. Despite the sustained effort to make IG methods more data-efficient, it remains an open question how to select a training data subset that can theoretically and practically perform on par with the full dataset. Here we develop CRAIG, a method to select a weighted subset (or coreset) of training data that closely estimates the full gradient by maximizing a submodular function. We prove that applying IG to this subset is guaranteed to converge to the (near)optimal solution with the same convergence rate as that of IG for convex optimization. As a result, CRAIG achieves a speedup that is inversely proportional to the size of the subset. To our knowledge, this is the first rigorous method for data-efficient training of general machine learning models. Our extensive set of experiments show that CRAIG, while achieving practically the same solution, speeds up various IG methods by up to 6x for logistic regression and 3x for training deep neural networks.
<br><br>

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @InProceedings{pmlr-v119-mirzasoleiman20a,
  title = 	 {Coresets for Data-efficient Training of Machine Learning Models},
  author =       {Mirzasoleiman, Baharan and Bilmes, Jeff and Leskovec, Jure},
  booktitle = 	 {Proceedings of the 37th International Conference on Machine Learning},
  pages = 	 {6950--6960},
  year = 	 {2020},
  editor = 	 {III, Hal Daumé and Singh, Aarti},
  volume = 	 {119},
  series = 	 {Proceedings of Machine Learning Research},
  month = 	 {13--18 Jul},
  publisher =    {PMLR},
  pdf = 	 {http://proceedings.mlr.press/v119/mirzasoleiman20a/mirzasoleiman20a.pdf},
  url = 	 {https://proceedings.mlr.press/v119/mirzasoleiman20a.html}
  }
</code></pre>
{% endraw %}
</details>
</blockquote></details>



<details><summary><b>Towards Trustworthy and Aligned Machine Learning: A Data-centric Survey with Causality Perspectives</b> 
<br>
&emsp;<i>Haoyang Liu, Maheep Chaudhary, Haohan Wang</i>
<br>
&emsp;<i>arXiv, 2023</i>
<br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://arxiv.org/abs/2307.16851">Paper</a>]
<br>
<br>
</summary>
  <blockquote> <b>Abstract:</b> The trustworthiness of machine learning has emerged as a critical topic in the field, encompassing various applications and research areas such as robustness, security, interpretability, and fairness. The last decade saw the development of numerous methods addressing these challenges. In this survey, we systematically review these advancements from a data-centric perspective, highlighting the shortcomings of traditional empirical risk minimization (ERM) training in handling challenges posed by the data.
Interestingly, we observe a convergence of these methods, despite being developed independently across trustworthy machine learning subfields. Pearl's hierarchy of causality offers a unifying framework for these techniques. Accordingly, this survey presents the background of trustworthy machine learning development using a unified set of concepts, connects this language to Pearl's causal hierarchy, and finally discusses methods explicitly inspired by causality literature. We provide a unified language with mathematical vocabulary to link these methods across robustness, adversarial robustness, interpretability, and fairness, fostering a more cohesive understanding of the field.
Further, we explore the trustworthiness of large pretrained models. After summarizing dominant techniques like fine-tuning, parameter-efficient fine-tuning, prompting, and reinforcement learning with human feedback, we draw connections between them and the standard ERM. This connection allows us to build upon the principled understanding of trustworthy methods, extending it to these new techniques in large pretrained models, paving the way for future methods. Existing methods under this perspective are also reviewed.
Lastly, we offer a brief summary of the applications of these methods and discuss potential future aspects related to our survey. For more information, please visit http://trustai.one.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @article{liu2023towards,
  title={Towards Trustworthy and Aligned Machine Learning: A Data-centric Survey with Causality Perspectives},
  author={Liu, Haoyang and Chaudhary, Maheep and Wang, Haohan},
  journal={arXiv preprint arXiv:2307.16851},
  year={2023}
}</code></pre>
{% endraw %}
</details>
</blockquote>
</details>