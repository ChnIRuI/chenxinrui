---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

# 👋🏻 Welcome!

Hello! I am **Xinrui Chen (陈新睿)**, a master's student in Artificial Intelligence at the **Hangzhou Institute for Advanced Study, University of Chinese Academy of Sciences (UCAS)**, under the supervision of Professor [Ou Wu](https://www.scholat.com/wuou). I received my bachelor's degree in Software Engineering from **Northeastern University**.

My research interests include **LLM post-training, agentic reinforcement learning, and recursive self-improvement (RSI)**, with a focus on efficient adaptation, model safety, and knowledge updating. My work has been accepted at **NeurIPS, ICLR, and EMNLP**. I am also exploring how agentic systems can enable continuous model improvement through interaction and experience.

**I am currently seeking industry opportunities and Ph.D. positions in large language models. Please feel free to contact me via email ([chenxinrui25@mails.ucas.ac.cn](mailto:chenxinrui25@mails.ucas.ac.cn), [chnirui224@gmail.com](mailto:chnirui224@gmail.com)).**

# 🔥 News

- *2026.10*: 🏅 Received the **National Scholarship (Graduate)** at UCAS.
- *2026.09*: 🎉🎉 **Two papers** accepted at **NeurIPS 2026**. *(Efficient LLM Fine-tuning & Data-centric Adaptation)*
- *2026.08*: 🎉🎉 **Two papers** accepted at **EMNLP 2026**. *(Safe LLM Fine-tuning & Relation Replacement Editing)*
- *2026.01*: 🎉 **One paper** accepted at **ICLR 2026**. *(Robust LLM Unlearning & Model Safety)*
- *2025.09*: 🎓 Began my M.S. studies in Artificial Intelligence at the **HIAS, UCAS**.
- *2025.06*: 🎓 Graduated from **Northeastern University** with a B.Eng. in Software Engineering.
- *2024.09*: 🎉 Received a recommendation-based admission to the **HIAS, UCAS**, to pursue graduate study under Prof. Ou Wu.

# 📝 Publications

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">NeurIPS 2026</div>
<img src='images/dualsft.png' alt="DualSFT framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

**[One Algorithm, Two Goals: Dual Scoring for Parameter and Data Selection in LLM Fine-Tuning](https://neurips.cc/virtual/2026/loc/sydney/poster/149252) (<span style="color: #d93025; font-weight: bold;">CCF-A</span>, First Author)**

**Xinrui Chen**, Liu Yang, Ou Wu<sup>*</sup>

**Keywords:** Efficient Fine-tuning · Joint Data–Parameter Selection

- Proposed **DualSFT**, a one-shot dual-scoring framework that jointly selects trainable parameters and training samples under a shared validation objective, deriving both selection signals from a unified gradient-interaction matrix.

</div>
</div>

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">ICLR 2026</div>
<img src='images/port.png' alt="PoRT framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

**[Robust LLM Unlearning via Post Judgment and Multi-round Thinking](https://proceedings.iclr.cc/paper_files/paper/2026/hash/72c12e48c6135762f56bf188cd2479d2-Abstract-Conference.html) (<span style="color: #d93025; font-weight: bold;">CCF-A</span>, First Author)**

**Xinrui Chen**, Xu Cao, Jianhao Zhang, Pinlong Zhao, Di Gao, Ou Wu<sup>*</sup>

**Keywords:** Robust Unlearning · Adversarial Defense

- Proposed **PoRT**, a robust unlearning framework that integrates dynamic input cleaning, joint post-judgment of queries and responses, and selective multi-round self-correction to defend against adversarial attacks.

</div>
</div>

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">EMNLP 2026</div>
<img src='images/dualselect.png' alt="DualSelect framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

**[Two to Tango: Coupled Task–Reference Selection for Safe LLM Fine-Tuning](https://aclanthology.org/2026.emnlp-main.862/) (<span style="color: #d93025; font-weight: bold;">CCF-B</span>, First Author)**

**Xinrui Chen**, Jianhao Zhang, Ou Wu<sup>*</sup>, Di Gao

**Keywords:** Safe Fine-tuning · Task–Reference Selection

- Proposed **DualSelect**, a coupled task–reference selection framework that identifies task-conditioned safety references and selects compatible task samples through entropy-regularized scoring and reference-gradient correction.

</div>
</div>

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">EMNLP 2026</div>
<img src='images/r2-edit.png' alt="R2Edit framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

**[R²Edit: Mastering Relation Replacement Editing via Target-Smoothed Forgetting and Self-Paced Learning](https://aclanthology.org/2026.emnlp-main.869/) (<span style="color: #d93025; font-weight: bold;">CCF-B</span>, Co-first Author)**

Xu Cao<sup>‡</sup>, **Xinrui Chen**<sup>‡</sup>, Qing Liu, Mengyang Li, Ou Wu<sup>*</sup>, Yi Du

**Keywords:** Knowledge Editing · Relation Replacement

- Proposed **R²Edit** and ReEditBench for relation-replacement editing, combining target-smoothed forgetting to suppress obsolete relations with curriculum-guided self-paced learning to introduce new relations.

</div>
</div>

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">NeurIPS 2026</div>
<img src='images/drive.png' alt="DRIVE framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

**[DRIVE: Fine-tuning via Data Contribution- and Diversity-aware Weighting with Prior Regularization](https://neurips.cc/virtual/2026/loc/sydney/poster/151453) (<span style="color: #d93025; font-weight: bold;">CCF-A</span>, Second Author)**

Qing Liu, **Xinrui Chen**, Yi Du<sup>*</sup>, Ou Wu, Weiyao Zhu

**Keywords:** Data-centric Fine-tuning · Diversity-aware Weighting

- Proposed **DRIVE**, a differentiable data-weighting framework that integrates Shapley-based contribution decomposition, covariance-based diversity modeling, and prior regularization to balance knowledge retention and task adaptation.

</div>
</div>

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">Under Review</div>
<img src='images/hilore.png' alt="HiLoRe framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

**[HiLoRe: What to Store, Compress, or Recompute for Efficient GRPO Training](https://arxiv.org/abs/2609.33570) (First Author)**

**Xinrui Chen**, Mengyang Li, Ou Wu<sup>*</sup>, Ji Zhang

**Keywords:** Efficient GRPO · Activation Management

- Proposed **HiLoRe**, an update-aware activation-recovery framework for GRPO training that coordinates high-precision storage, low-precision compression, and deterministic recomputation under memory and approximation-risk constraints.

</div>
</div>

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">Under Review</div>
<img src='images/SID.png' alt="SID framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

**Sample-wise Interactions: Dissecting the Stability-Plasticity Dilemma in LLM Fine-tuning** **(First Author)**

**Xinrui Chen**

**Keywords:** Sample-wise Interactions · Stability–Plasticity

- Proposed **SID**, a sample-wise interaction framework for characterizing how individual training examples jointly shape optimization stability and task adaptation during LLM fine-tuning.

</div>
</div>

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">Under Review</div>
<img src='images/pask.png' alt="PASK framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

**[Parser Transitions Already Reveal Structural Responsibility: KV Persistence for Structured Generation](https://arxiv.org/abs/2608.28276) (Second Author, Corresponding Author)**

Linze Wu, **Xinrui Chen**<sup>*</sup>

**Keywords:** LLM Inference · KV Cache Optimization · Structured Generation

- Proposed **PASK**, a parser-aware KV-persistence framework that reuses parser transitions to identify structurally critical tokens and allocate KV retention across layer groups under a fixed memory budget.

</div>
</div>

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">Under Review</div>
<img src='images/bridge.png' alt="BRIDGE framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

**[Token Utility Is Selection-Conditioned: Coupled Selection of Prompt Context and Response Supervision for Instruction Tuning](https://arxiv.org/abs/2609.22943) (Second Author)**

Can Wu, **Xinrui Chen**, Ou Wu<sup>*</sup>, Yi Du

**Keywords:** Instruction Tuning · Prompt–Response Selection

- Proposed **BRIDGE**, a coupled token-selection framework that jointly selects prompt context and response supervision by modeling selection-conditioned utility under the opposite side's retained subset, with budgeted alternating selection and structure-aware projection.

</div>
</div>

# 📝 Patents

- **A Large Language Model Unlearning Method, System, and Medium Based on Post-filtering and Repeated Thinking**, <span style="color: #d93025; font-weight: bold;">Invention Patent Application (Accepted)</span>, P.R. China Patent Application No. 202610119333.9 (2026.01).

  **Xinrui Chen**, Ou Wu

- **A Lightweight LLM Inference Method, System, and Medium Based on Dictionary-level Token Masking**, <span style="color: #d93025; font-weight: bold;">Invention Patent Application (Accepted)</span>, P.R. China Patent Application No. 202610607888.8 (2026.05).

  Ou Wu, Shuxin Liu, **Xinrui Chen**, Yi Du

# 🏅 Honors and Awards

- *2026.10*, **National Scholarship (Graduate)**.
- *2026.09*, First-Class Scholarship, University of Chinese Academy of Sciences (UCAS).
- *2026.06*, Outstanding Model Three-Good Student Award, University of Chinese Academy of Sciences (UCAS).
- *2026.06*, Three-Good Student Award, University of Chinese Academy of Sciences (UCAS).
- *2024.05*, Honorable Mention, Interdisciplinary Contest in Modeling (ICM).
- *2024.01*, Meritorious Winner, 9th ShuWei Cup International Undergraduate Mathematical Contest in Modeling.
- *2023.09*, Second-Class Scholarship, Northeastern University.
- *2023.09*, Outstanding Student, Northeastern University.
- *2023.09*, Third-Class Scholarship, Beike.
- *2023.06*, Third Prize (Type C), National English Competition for College Students (NECCS).
- *2023.05*, Honorable Mention, Mathematical Contest in Modeling (MCM).
- *2023.05*, Third Place, Northeastern University Campus Debate Competition.
- *2022.09*, **National Scholarship (Undergraduate)**.
- *2022.09*, First-Class Scholarship, Northeastern University.
- *2022.09*, Academic Excellence Award, School of Software, Northeastern University.
- *2022.09*, Outstanding Model Communist Youth League Member, Northeastern University.

# 📖 Education

- **2025.09 – 2028.06 (Expected):** M.S. in Artificial Intelligence, University of Chinese Academy of Sciences.
- **2021.09 – 2025.06:** B.Eng. in Software Engineering, Northeastern University.

# 💼 Internship Experience

- *Oct. 2024 – Jan. 2025*, Software Development Intern, **CARIZON (Beijing) Technology Co., Ltd.**

