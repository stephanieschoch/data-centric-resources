---
layout: default
title: Natural Language Data
nav_order: 3
has_children: false
has_toc: false
---

# Natural Language Data

Contains papers related to evaluating natural language data (e.g. identifying annotation artifacts, designing benchmark datasets).

## Annotation Errors

<details><summary><b>ActiveAED: A Human in the Loop Improves Annotation Error Detection</b> <br>
&emsp;<i>Leon Weber, Barbara Plank</i><br>
&emsp;<i>Findings of the Association for Computational Linguistics (ACL), 2023</i><br>&emsp;
[<a target="_blank" rel="noopener noreferrer" href="https://aclanthology.org/2023.findings-acl.562/">Paper</a>]
[<a target="_blank" rel="noopener noreferrer" href="https://github.com/mainlp/ActiveAED">Code</a>]
<br><br></summary>

<blockquote> <b>Abstract:</b> Manually annotated datasets are crucial for training and evaluating Natural Language Processing models. However, recent work has discovered that even widely-used benchmark datasets contain a substantial number of erroneous annotations. This problem has been addressed with Annotation Error Detection (AED) models, which can flag such errors for human re-annotation. However, even though many of these AED methods assume a final curation step in which a human annotator decides whether the annotation is erroneous, they have been developed as static models without any human-in-the-loop component. In this work, we propose ActiveAED, an AED method that can detect errors more accurately by repeatedly querying a human for error corrections in its prediction loop. We evaluate ActiveAED on eight datasets spanning five different tasks and find that it leads to improvements over the state of the art on seven of them, with gains of up to six percentage points in average precision.
<br><br>

<!--
<details><summary><b>Notes</b></summary>TEXT
<br><br></details>
-->

<details><summary><b>Bibtex</b></summary>
{% raw %}
<pre><code> @inproceedings{weber-plank-2023-activeaed,
    title = "{A}ctive{AED}: A Human in the Loop Improves Annotation Error Detection",
    author = "Weber, Leon  and
      Plank, Barbara",
    editor = "Rogers, Anna  and
      Boyd-Graber, Jordan  and
      Okazaki, Naoaki",
    booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.findings-acl.562",
    doi = "10.18653/v1/2023.findings-acl.562",
    pages = "8834--8845"
    } </code></pre>
{% endraw %}
</details>
</blockquote></details>