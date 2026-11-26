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

I am a master's student in Artificial Intelligence at the **University of Chinese Academy of Sciences (UCAS)**. I received my bachelor's degree in Software Engineering from **Northeastern University**.

My research focuses on **efficient post-training, safety, and knowledge updating for large language models (LLMs)**. My interests include data- and parameter-efficient fine-tuning, robust unlearning, knowledge editing, and memory-efficient LLM training.

# 🔬 Research Interests

- **Efficient LLM Post-training:** Data- and parameter-efficient adaptation, coordinated sample and parameter selection, and resource-aware optimization.
- **LLM Safety and Unlearning:** Robust removal of undesired knowledge and harmful behaviors while preserving general capabilities.
- **Knowledge Editing and Updating:** Reliable factual updates and relation replacement with controlled side effects.
- **Efficient LLM Training:** Memory- and computation-aware optimization for reinforcement-learning-based LLM training.

# 🔥 News

- Research papers on efficient LLM fine-tuning, robust unlearning, and safe model adaptation have been accepted at **NeurIPS, ICLR, and EMNLP**. See the publication list below for details.

# 📝 Publications

## Accepted

<!--
Add paper thumbnails under images/papers/ using the exact filenames referenced below.
Recommended: landscape images (16:9), at least 800 px wide, with a consistent visual style.
Use a framework overview, teaser figure, or representative result figure for each paper.
-->

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">NeurIPS · Accepted</div><img src='images/papers/dualsft.png' alt="DualSFT framework overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**One Algorithm, Two Goals: Dual Scoring for Parameter and Data Selection in LLM Fine-Tuning**

**Xinrui Chen**, L. Yang, et al. · **First Author**

Introduces **DualSFT**, a one-shot framework that jointly selects trainable parameters and training samples under a shared validation objective. Parameter importance and sample utility are derived from column-wise and row-wise aggregation of a shared gradient-interaction matrix. Confidence-weighted self-distillation further helps mitigate forgetting without access to pre-training data.

- **Result:** Under matched budgets of 5% trainable parameters and 10% training data, DualSFT improves the combined task-adaptation and general-capability score on Magicoder over the strongest same-budget sequential combination by **2.46**, **2.59**, and **3.22 percentage points** on Llama-3.2-3B, Gemma-3-4B, and Qwen-3.5-9B, respectively.

<!-- Add Paper / Project / Code links here when public URLs are available. -->

</div></div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICLR · Accepted</div><img src='images/papers/port.png' alt="PoRT framework overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Robust LLM Unlearning via Post Judgment and Multi-round Thinking**

**Xinrui Chen**, X. Cao, et al. · **First Author**

Proposes **PoRT**, a parameter-free robust unlearning framework that dynamically cleans inputs, jointly judges questions and answers, and triggers multi-round self-correction for low-confidence outputs.

- **Result:** Under noisy-prefix attacks on WMDP, the hazardous-biology knowledge accuracy of Qwen1.5-14B-Chat is **25.3%**, close to the 25% random level and below ECO's 67.0%. Zephyr-7B retains **58.9%** MMLU accuracy, matching the original model.

<!-- Add Paper / Project / Code links here when public URLs are available. -->

</div></div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">EMNLP · Accepted</div><img src='images/papers/dualselect.png' alt="DualSelect framework overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Two to Tango: Coupled Task–Reference Selection for Safe LLM Fine-Tuning**

**Xinrui Chen**, J. Zhang, et al. · **First Author**

Proposes **DualSelect**, which couples task-data selection with safety-reference selection. It selects safety references according to retention loss and gradient conflict, then selects task samples compatible with the reference-gradient direction. Entropy-regularized scoring, delayed refresh, and gradient correction help control overhead and constrain harmful updates.

- **Result:** On REDORCA, Safety Avg. improves by **5.10–5.80 percentage points** over the strongest baseline across three 1B–8B models. For Llama-3-8B, the attack success rate decreases from **52.8% to 15.8%**, with a false refusal rate of **5.8%**.

<!-- Add Paper / Project / Code links here when public URLs are available. -->

</div></div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">EMNLP · Accepted</div><img src='images/papers/r2-edit.png' alt="R2 Edit framework overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**R2 Edit: Mastering Relation Replacement Editing via Target-Smoothed Forgetting and Self-Paced Learning**

X. Cao*, **Xinrui Chen***, et al. · **Co-first Author**

Introduces **ReEditBench**, a benchmark for relation-replacement editing, and a method that combines target-smoothed forgetting with self-paced learning. The approach first suppresses the old relation and then injects the new relation from easier to harder examples.

- **Result:** On LLaMA3, relation-replacement success improves from **52.18% to 81.71%** over AlphaEdit. On GPT2-XL, the old-relation retention rate changes from **91.31% to 48.78%**.

<!-- Add Paper / Project / Code links here when public URLs are available. -->

</div></div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">NeurIPS · Accepted</div><img src='images/papers/drive.png' alt="DRIVE framework overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**DRIVE: Fine-tuning via Data Contribution- and Diversity-aware Weighting with Prior Regularization**

Q. Liu, **Xinrui Chen**, et al. · **Second Author**

Studies data-aware fine-tuning through a weighting strategy that considers sample contribution and diversity together with prior regularization.

<!-- Add Paper / Project / Code links here when public URLs are available. -->

</div></div>

## Under Review

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Under Review</div><img src='images/papers/hilore.png' alt="HiLoRe framework overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**HiLoRe: What to Store, Compress, or Recompute for Efficient GRPO Training**

**Xinrui Chen** · **First Author**

Studies the trade-off between activation memory and recomputation overhead in GRPO training. HiLoRe uses policy-update signals to estimate approximation risk and jointly schedules high-precision storage, low-precision compression, and recomputation under memory and error budgets.

- **Result:** With a peak-memory budget no greater than 1.10× GC at a response length of 2K, throughput improves by up to **13.5%** over GC and **7.9%** over the fastest comparator. Across five configurations, the average downstream score differs from GC by less than **0.6 percentage points**.

</div></div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Under Review</div><img src='images/papers/sid.png' alt="SID framework overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Sample-wise Interactions: Dissecting the Stability-Plasticity Dilemma in LLM Fine-tuning**

**Xinrui Chen** · **First Author**

Studies sample-wise interactions during LLM fine-tuning and their role in the stability–plasticity trade-off.

</div></div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Under Review</div><img src='images/papers/pask.png' alt="PASK framework overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Parser Transitions Already Reveal Structural Responsibility: KV Persistence for Structured Generation**

**Xinrui Chen** · **Corresponding Author**

Investigates parser-transition signals as indicators of structural responsibility for KV-cache persistence in structured generation.

</div></div>

# 🎖 Honors and Awards

- **National Scholarship**
- **Outstanding Three-Good Student Award**
- **First-Class Scholarship**
- **H Award**, International Undergraduate Mathematical Contest in Modeling (2023 and 2024)
- **Third Place**, Northeastern University Campus Debate Competition

# 📖 Education

- **2025.09 – 2028.06 (Expected):** M.S. in Artificial Intelligence, University of Chinese Academy of Sciences.
- **2021.09 – 2025.06:** B.Eng. in Software Engineering, Northeastern University.

# 🧰 Technical Skills

- **Programming:** Python, PyTorch, Linux, and Git.
- **LLM Training:** Supervised fine-tuning (SFT), direct preference optimization (DPO), group relative policy optimization (GRPO), and LoRA-based parameter-efficient fine-tuning.
- **Training Frameworks:** Transformers, PEFT, LLaMAFactory, and DeepSpeed; experience with gradient accumulation and multi-GPU FSDP training.
- **Parallelism:** Familiar with the basic mechanisms and use cases of tensor parallelism (TP), sequence parallelism (SP), and pipeline parallelism (PP).

# 📧 Contact

- **Email:** [chenxinrui25@mails.ucas.ac.cn](mailto:chenxinrui25@mails.ucas.ac.cn)
- **GitHub:** [CHNIRUI-Code](https://github.com/CHNIRUI-Code)
