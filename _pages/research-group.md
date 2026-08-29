---
layout: page
title: Research Group
permalink: /research-group/
description: The Yukun Ma Research Group develops econometric methods for reliable inference with dependent data, machine learning, weak identification, and weak overlap.
keywords: Yukun Ma Research Group, Principal Investigator, PI, econometrics research group, econometric theory, causal inference, robust inference, machine learning, weak identification, weak overlap
nav: true
nav_order: 3
---

<div class="research-group-intro">
  <p class="eyebrow">Yukun Ma Research Group</p>
  <h2>Econometrics for difficult data</h2>
  <p>Many empirical projects now combine exactly the features that make conventional inference fragile: flexible machine learning, complicated dependence, weak instruments, or limited overlap. I lead a research program that asks what researchers can still learn—and how honestly they can quantify uncertainty—when the textbook assumptions are at their weakest.</p>
</div>

The group is small by design right now: I am the Principal Investigator, I work with coauthors across institutions, and student members will be added here as they join. On this page, “we” means the research program being built through those collaborations—not a large lab hiding behind a plural pronoun.

## What we work on

<div class="research-program-grid">
  <section class="research-topic">
    <p class="topic-number">01</p>
    <h3>Machine learning when observations are connected</h3>
    <p>Cross-fitting and standard errors are straightforward when observations are independent. Economic data often are not: workers share firms and regions, countries form pairs, and markets are linked. We develop double/debiased machine-learning methods that remain valid under multiway clustering and dyadic dependence.</p>
    <p class="research-links">
      <a href="https://doi.org/10.1080/07350015.2021.1895815">Multiway DML paper</a>
      <a href="https://arxiv.org/abs/1909.03489">arXiv</a>
      <a href="https://docs.doubleml.org/stable/api/api.html">Python</a>
      <a href="https://docs.doubleml.org/r/stable/">R</a>
      <a href="https://doi.org/10.1017/S0266466625100273">Dyadic DML paper</a>
      <a href="https://drive.google.com/file/d/14Ph9ne_-4070ambP0mw4IEwRyQmyieCg/view?usp=sharing">Replication package</a>
    </p>
  </section>

  <section class="research-topic">
    <p class="topic-number">02</p>
    <h3>Causal inference with weak instruments and many controls</h3>
    <p>Researchers often want to use rich covariates and machine learning while the instrument itself may be weak. Our work combines the Anderson–Rubin idea with orthogonalization and double machine learning, producing inference for the local average treatment effect that does not pretend identification is stronger than it is.</p>
    <p class="research-links">
      <a href="https://doi.org/10.1016/j.jeconom.2026.106302">Journal of Econometrics</a>
      <a href="https://arxiv.org/abs/2302.09756">arXiv</a>
      <a href="https://www.sciencedirect.com/science/article/pii/S0304407626001235">Article page</a>
    </p>
  </section>

  <section class="research-topic">
    <p class="topic-number">03</p>
    <h3>Treatment effects when comparable units are scarce</h3>
    <p>When treated and comparison units look very different, conventional weighting estimators can become noisy or unstable. We study how trimming and bias correction can work together, preserving double robustness while making estimation more useful under weak overlap.</p>
    <p class="research-links">
      <a href="https://arxiv.org/abs/2304.08974">Working paper</a>
      <a href="https://arxiv.org/pdf/2304.08974">PDF</a>
      <a href="https://psantanna.com/files/MSSU2026.pdf">April 2026 version</a>
    </p>
  </section>
</div>

## Selected research outcomes

<div class="research-outcomes">
  <article class="paper-card">
    <p class="paper-status">Journal of Business &amp; Economic Statistics · 2022</p>
    <h3><a href="https://doi.org/10.1080/07350015.2021.1895815">Multiway Cluster Robust Double/Debiased Machine Learning</a></h3>
    <p>Introduces multiway cross-fitting, a multiway DML estimator, and cluster-robust standard errors for settings such as market demand data with dependence along more than one dimension.</p>
    <p>With <a href="https://sites.google.com/view/haroldchiang/home">Harold D. Chiang</a>, <a href="https://sites.google.com/site/kkatostat/home">Kengo Kato</a>, and <a href="https://sites.google.com/site/yuyasasaki/">Yuya Sasaki</a>.</p>
    <p class="research-links">
      <a href="https://www.tandfonline.com/doi/abs/10.1080/07350015.2021.1895815">Published article</a>
      <a href="https://www.tandfonline.com/doi/suppl/10.1080/07350015.2021.1895815?scroll=top">R code</a>
      <a href="https://drive.google.com/file/d/1G2Nn6LzmICQwtC02Z0H8Truo7vTPwutp/view">Stata code</a>
    </p>
  </article>

  <article class="paper-card">
    <p class="paper-status">Econometric Theory · First View, 2026</p>
    <h3><a href="https://doi.org/10.1017/S0266466625100273">Double/Debiased Machine Learning for Dyadic Data</a></h3>
    <p>Develops dyadic cross-fitting for network and pair-level data and applies the method to the determinants of free trade agreements.</p>
    <p>With <a href="https://sites.google.com/view/haroldchiang/home">Harold D. Chiang</a>, <a href="https://joelrodrigue.com/">Joel B. Rodrigue</a>, and <a href="https://sites.google.com/site/yuyasasaki/">Yuya Sasaki</a>.</p>
    <p class="research-links">
      <a href="https://www.cambridge.org/core/journals/econometric-theory/article/doubledebiased-machine-learning-for-dyadic-data/463CA7664A3252892656F934591B54E3">Open-access article</a>
      <a href="https://drive.google.com/file/d/14Ph9ne_-4070ambP0mw4IEwRyQmyieCg/view?usp=sharing">Code &amp; data</a>
    </p>
  </article>

  <article class="paper-card">
    <p class="paper-status">Journal of Econometrics · 2026</p>
    <h3><a href="https://doi.org/10.1016/j.jeconom.2026.106302">Identification-Robust Inference for the LATE with High-Dimensional Covariates</a></h3>
    <p>Builds an orthogonalized Anderson–Rubin procedure for LATE with many controls, with an application to railroad access and urban population growth.</p>
    <p class="research-links">
      <a href="https://www.sciencedirect.com/science/article/pii/S0304407626001235">Published article</a>
      <a href="https://arxiv.org/abs/2302.09756">arXiv</a>
    </p>
  </article>

  <article class="paper-card">
    <p class="paper-status">Working paper · revised April 2026</p>
    <h3><a href="https://arxiv.org/abs/2304.08974">Doubly Robust Estimators with Weak Overlap</a></h3>
    <p>Uses trimming with bias correction to retain double robustness across unconfoundedness, instrumental-variables, and difference-in-differences designs.</p>
    <p>With <a href="https://psantanna.com/">Pedro H. C. Sant’Anna</a>, <a href="https://sites.google.com/site/yuyasasaki/">Yuya Sasaki</a>, and <a href="https://uratakuya.github.io/">Takuya Ura</a>.</p>
    <p class="research-links">
      <a href="https://arxiv.org/pdf/2304.08974">Latest PDF</a>
      <a href="https://ideas.repec.org/p/arx/papers/2304.08974.html">RePEc</a>
    </p>
  </article>
</div>

The full publication list is on the [Research page]({% link _pages/research.md %}) and my [Google Scholar profile](https://scholar.google.com/citations?user=MFra9aUAAAAJ). Code and replication materials are linked next to each paper whenever they are publicly available.

## People and collaboration

<div class="group-person">
  <div>
    <p class="person-role">Principal Investigator</p>
    <h3><a href="{% link _pages/about.md %}">Yukun Ma</a></h3>
    <p>Assistant Professor in the <a href="https://www.sas.rochester.edu/eco/">Department of Economics</a>, University of Rochester<br>Joint appointment, <a href="https://www.hajim.rochester.edu/dsc/">Goergen Institute for Data Science and Artificial Intelligence</a></p>
    <p><a href="{% link _pages/cv.md %}">CV</a> · <a href="https://scholar.google.com/citations?user=MFra9aUAAAAJ">Google Scholar</a> · <a href="https://github.com/yukunma">GitHub</a> · <a href="mailto:yma69@ur.rochester.edu">Email</a></p>
  </div>
</div>

Most projects grow out of long conversations with collaborators rather than a fixed lab pipeline. Coauthors are credited on the relevant papers above; they are collaborators on those projects, not automatically members of the research group.

## For students

If you are interested in working with me, you do not need to arrive with a finished theorem or a perfectly specified project. A good starting point is a concrete empirical problem where the usual inference feels too confident, or a methodological question about dependence, high dimensionality, weak instruments, or weak overlap.

Student members and their projects will be added to this page as they join. For now, the best way to start a conversation is to read one of the papers above and email me at [yma69@ur.rochester.edu](mailto:yma69@ur.rochester.edu) with the question that stayed with you.
