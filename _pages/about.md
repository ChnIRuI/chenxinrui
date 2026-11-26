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

I am currently a master's student in Artificial Intelligence at the **University of Chinese Academy of Sciences (UCAS)**. I received my bachelor's degree in Software Engineering from **Northeastern University**.

My research focuses on **efficient post-training, safety, and knowledge updating for Large Language Models (LLMs)**. My interests include data- and parameter-efficient fine-tuning, robust unlearning, knowledge editing, and efficient LLM training and inference.

# 🔬 Research Interests

- **Efficient LLM Post-training:** Data- and parameter-efficient adaptation, coordinated sample and parameter selection.
- **LLM Safety and Unlearning:** Robust unlearning and safety preservation under adversarial attacks.
- **Knowledge Editing:** Reliable factual updating and relation replacement with controlled side effects.
- **Efficient LLM Training:** Memory- and computation-efficient optimization for LLM reinforcement learning.

# 🔥 News

- 2026: 🎉 Papers on efficient fine-tuning, robust unlearning, and safe LLM adaptation accepted at **NeurIPS, ICLR, and EMNLP**.

# 📝 Publications

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">NeurIPS 2026</div>
<img src='images/dualsft.png' alt="DualSFT framework" width="100%">
</div>
</div>

[One Algorithm, Two Goals: Dual Scoring for Parameter and Data Selection in LLM Fine-Tuning](https://arxiv.org/abs/2605.06166)

**Xinrui Chen**, Liu Yang, Ou Wu<sup>*</sup>

**[GitHub](https://github.com/ChnIRuI/DualSFT)**

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

<div style="text-align:right; margin-bottom:6px;">
<span class="badge">* Corresponding Author</span>
</div>

[Robust LLM Unlearning via Post Judgment and Multi-round Thinking](https://openreview.net/forum?id=GBTUVO9vkj)

**Xinrui Chen**, Xu Cao, Jianhao Zhang, Pinlong Zhao, Di Gao, Ou Wu<sup>*</sup>

**[GitHub](https://github.com/ChnIRuI/PoRT_LLM_Unlearning)**

- Proposed **PoRT**, a robust unlearning framework integrating dynamic input cleaning, confidence-aware post-judgment of questions and responses, and selective multi-round self-correction to defend against adversarial attacks.

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

<div style="text-align:right; margin-bottom:6px;">
<span class="badge">* Corresponding Author</span>
</div>

[Two to Tango: Coupled Task–Reference Selection for Safe LLM Fine-Tuning](https://aclanthology.org/2026.emnlp-main.862/)

**Xinrui Chen**, Jianhao Zhang, Ou Wu<sup>*</sup>, Di Gao

**[GitHub](https://github.com/ChnIRuI/DualSelect)**

- Proposed **DualSelect**, a coupled task–reference selection framework that identifies task-conditioned safety references and selects compatible task samples through entropy-regularized scoring and reference-gradient correction.

</div>
</div>

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">EMNLP 2026</div>
<img src='images/r2edit.png' alt="R2Edit framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

<div style="text-align:right; margin-bottom:6px;">
<span class="badge">* Equal Contribution</span>
<span class="badge">‡ Corresponding Author</span>
</div>

[R²Edit: Mastering Relation Replacement Editing via Target-Smoothed Forgetting and Self-Paced Learning](https://aclanthology.org/2026.emnlp-main.869/)

Xu Cao<sup>*†</sup>, **Xinrui Chen**<sup>*</sup>, Qing Liu, Mengyang Li, Ou Wu<sup>‡</sup>, Yi Du

**[GitHub](https://github.com/caoxu0109/R2Edit)**

- Proposed **R²Edit** and ReEditBench for relation-replacement editing, combining target-smoothed forgetting to suppress obsolete relations with curriculum-guided self-paced learning to introduce new relations.

<small><sup>*</sup> Equal contribution. <sup>†</sup> Work conducted during an internship at HIAS, UCAS. <sup>‡</sup> Corresponding author.</small>

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

<div style="text-align:right; margin-bottom:6px;">
<span class="badge">* Corresponding Author</span>
</div>

[DRIVE: Fine-tuning via Data Contribution- and Diversity-aware Weighting with Prior Regularization](https://arxiv.org/abs/2610.32501)

Qing Liu, **Xinrui Chen**, Yi Du<sup>*</sup>, Ou Wu, Weiyao Zhu

**[GitHub](https://github.com/luciabcd/DRIVE)**

- Proposed **DRIVE**, a unified differentiable data-weighting framework that integrates Shapley-based contribution decomposition, covariance-based diversity modeling, and prior regularization to balance knowledge retention and task adaptation.

</div>
</div>

# 📄 Under Review

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">Under Review</div>
<img src='images/hilore.png' alt="HiLoRe framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

<div style="text-align:right; margin-bottom:6px;">
<span class="badge">* Corresponding Author</span>
</div>

[HiLoRe: What to Store, Compress, or Recompute for Efficient GRPO Training](https://arxiv.org/abs/2609.33570)

**Xinrui Chen**, Mengyang Li, Ou Wu<sup>*</sup>, Ji Zhang

**[GitHub](https://github.com/ChnIRuI/HiLoRe)**

- Proposed **HiLoRe**, an update-aware activation-recovery framework for GRPO training that coordinates high-precision storage, low-precision compression, and deterministic recomputation under memory and approximation-risk constraints.

</div>
</div>

<div class='paper-box'>
<div class='paper-box-image'>
<div>
<div class="badge">Under Review</div>
<img src='images/sid.png' alt="SID framework" width="100%">
</div>
</div>
<div class='paper-box-text' markdown="1">

**Sample-wise Interactions: Dissecting the Stability-Plasticity Dilemma in LLM Fine-tuning**

**Xinrui Chen** · First Author

- Studies sample-wise interactions during LLM fine-tuning, analyzing how individual training examples jointly influence optimization stability and task adaptation.

<!-- Add the complete co-author list and author-role markers after confirmation. -->

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

<div style="text-align:right; margin-bottom:6px;">
<span class="badge">* Corresponding Author</span>
</div>

[Parser Transitions Already Reveal Structural Responsibility: KV Persistence for Structured Generation](https://arxiv.org/abs/2608.28276)

Linze Wu, **Xinrui Chen**<sup>*</sup>

- Proposed **PASK**, a parser-aware KV-persistence framework that reuses parser transitions to identify structurally critical tokens and allocate KV retention across layer groups under a fixed memory budget.

</div>
</div>

# 🎖 Honors and Awards

- National Scholarship.
- Outstanding Three-Good Student Award.
- First-Class Scholarship.
- H Award, International Undergraduate Mathematical Contest in Modeling (2023 and 2024).
- Third Place, Northeastern University Campus Debate Competition.

# 📖 Education

- **2025.09 – 2028.06 (Expected):** M.S. in Artificial Intelligence, University of Chinese Academy of Sciences.
- **2021.09 – 2025.06:** B.Eng. in Software Engineering, Northeastern University.

# 💻 Technical Skills

- **Programming:** Python, PyTorch, Linux, and Git.
- **LLM Training:** SFT, DPO, GRPO, and LoRA-based parameter-efficient fine-tuning.
- **Training Frameworks:** Transformers, PEFT, LLaMAFactory, and DeepSpeed; multi-GPU FSDP training.
- **Parallelism:** Tensor Parallelism (TP), Sequence Parallelism (SP), and Pipeline Parallelism (PP).

# 📧 Contact

- **Email:** [chenxinrui25@mails.ucas.ac.cn](mailto:chenxinrui25@mails.ucas.ac.cn)
- **GitHub:** [CHNIRUI-Code](https://github.com/CHNIRUI-Code)
