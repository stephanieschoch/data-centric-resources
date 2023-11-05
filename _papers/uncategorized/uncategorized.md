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