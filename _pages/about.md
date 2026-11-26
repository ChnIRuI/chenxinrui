---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<span class='anchor' id='about-me'></span>

I am an M.S. student in Artificial Intelligence at the University of Chinese Academy of Sciences (UCAS). My research focuses on efficient post-training of large language models, model safety, and knowledge updating. My current interests include data- and parameter-efficient fine-tuning, robust unlearning, knowledge editing, and efficient LLM training and inference.

# 🔬 Research Interests

- Efficient LLM Post-training and Fine-tuning
- Data- and Parameter-efficient Model Adaptation
- LLM Safety and Robust Unlearning
- Knowledge Editing and Updating
- Efficient LLM Training and Inference

# 📝 Publications

## Accepted Papers

1. **One Algorithm, Two Goals: Dual Scoring for Parameter and Data Selection in LLM Fine-Tuning**  
   X. Chen, L. Yang, et al.  
   *Advances in Neural Information Processing Systems (NeurIPS).* **Accepted; First author.**  
   DualSFT jointly selects trainable parameters and training data under a shared validation objective. It derives parameter importance and data utility from column- and row-wise aggregation of a shared gradient-interaction matrix, and combines the selection with confidence-weighted self-distillation. On Magicoder, it improves the combined task-adaptation and general-capability score over the strongest matched-budget sequential baseline by 2.46, 2.59, and 3.22 percentage points for Llama-3.2-3B, Gemma-3-4B, and Qwen-3.5-9B, respectively.

2. **Robust LLM Unlearning via Post Judgment and Multi-round Thinking**  
   X. Chen, X. Cao, et al.  
   *International Conference on Learning Representations (ICLR).* **Accepted; First author.**  
   PoRT addresses noisy and compound inputs that can bypass pre-filtering-based unlearning. It dynamically cleans inputs, jointly evaluates questions and answers, and triggers multi-round self-correction for low-confidence outputs without updating the main model parameters. Under noisy-prefix attacks on WMDP, Qwen1.5-14B-Chat achieves 25.3% hazardous biological-knowledge accuracy, close to the 25% random level; Zephyr-7B retains an MMLU score of 58.9%, matching the original model.

3. **Two to Tango: Coupled Task–Reference Selection for Safe LLM Fine-Tuning**  
   X. Chen, J. Zhang, et al.  
   *Empirical Methods in Natural Language Processing (EMNLP).* **Accepted; First author.**  
   DualSelect couples safety-reference selection with task-example selection. It selects safety references according to retention loss and gradient conflict with the current task, then selects compatible task examples along the reference-gradient direction. On REDORCA, it improves Safety Average by 5.10–5.80 percentage points over the strongest baseline across three models; for Llama-3-8B, it reduces attack success rate from 52.8% to 15.8%, with a 5.8% false refusal rate.

4. **R2 Edit: Mastering Relation Replacement Editing via Target-Smoothed Forgetting and Self-Paced Learning**  
   X. Cao*, X. Chen*, et al.  
   *Empirical Methods in Natural Language Processing (EMNLP).* **Accepted; Co-first author.**  
   This work introduces ReEditBench for relation-replacement editing and combines target-smoothed forgetting with self-paced learning: old relations are first suppressed, followed by progressively harder updates for new relations. Compared with AlphaEdit, the relation-replacement success rate on LLaMA3 increases from 52.18% to 81.71%. On GPT2-XL, the old-relation retention rate decreases from 91.31% to 48.78%, while maintaining generalization to new relations.

5. **DRIVE: Fine-tuning via Data Contribution- and Diversity-aware Weighting with Prior Regularization**  
   Q. Liu, X. Chen, et al.  
   *Advances in Neural Information Processing Systems (NeurIPS).* **Accepted; Second author.**

## Manuscripts Under Review

1. **HiLoRe: What to Store, Compress, or Recompute for Efficient GRPO Training**  
   **First author; Under review.**  
   HiLoRe uses policy-update signals to estimate approximation risk and jointly schedules high-precision storage, low-precision compression, and recomputation under memory and error budgets. With 2K response tokens and peak memory no greater than 1.10× that of GC, it achieves up to 13.5% higher throughput than GC and 7.9% higher throughput than the fastest comparator. Across five configurations, its average downstream score differs from GC by less than 0.6 percentage points.

2. **Sample-wise Interactions: Dissecting the Stability-Plasticity Dilemma in LLM Fine-tuning**  
   **First author; Under review.**

3. **Parser Transitions Already Reveal Structural Responsibility: KV Persistence for Structured Generation**  
   **Corresponding author; Under review.**

# 🎓 Education

- **M.S. in Artificial Intelligence**, University of Chinese Academy of Sciences (UCAS), September 2025 – June 2028.
- **B.Eng. in Software Engineering**, Northeastern University, China, September 2021 – June 2025.

# 🏆 Honors and Awards

- National Scholarship.
- Outstanding Student Award.
- First-Class Scholarship.
- H Award, International Mathematical Modeling Challenge (2023 and 2024).
- Third Place, Northeastern University Campus Debate Competition.

# 💻 Technical Skills

- **Programming:** Python, PyTorch, Linux, and Git.
- **LLM training:** Supervised fine-tuning (SFT), direct preference optimization (DPO), group relative policy optimization (GRPO), and LoRA-based parameter-efficient fine-tuning.
- **Frameworks:** Transformers, PEFT, LLaMAFactory, DeepSpeed, and FSDP.
- **Parallelism:** Tensor parallelism, sequence parallelism, and pipeline parallelism.
