# Awesome Affective Intelligence in Multimodal Large Language Models

A curated bibliography of **affective intelligence in multimodal large language models (MLLMs)**, maintained by **Yali Fu**.

[Survey manuscript repository](https://github.com/jindongli-Ai/2026_Survey_Affective-Intelligence-in-MLLMs)

**Repository resources:** [Canonical papers.csv](papers.csv) · [Taxonomy validation & method matrix](TAXONOMY-VALIDATION.md) · [Benchmark coverage](BENCHMARK-COVERAGE.md) · [2026 research watchlist](2026-RESEARCH-WATCHLIST.md) · [Literature curation protocol](CURATION.md)

**Latest literature expansion (2026-10-29):** added 20 verified records from EMNLP/Findings, ACL, ICLR, EACL and arXiv, including [SoVTR](https://aclanthology.org/2026.findings-emnlp.1807/), [UniMER](https://aclanthology.org/2026.emnlp-main.1611/), [TMPO](https://proceedings.iclr.cc/paper_files/paper/2026/hash/89ab43b626b480347dbaccda7be8aedb-Abstract-Conference.html), and [HMER](https://arxiv.org/abs/2609.11154). `New-verified` means bibliographic identity and public abstract checked; it does **not** mean full-text review.

The collection spans affective evidence modeling, affective training and optimization, inference-time emotion reasoning, empathetic interaction, benchmarks, and adjacent research. The taxonomy is **provisional** and will be refined paper by paper.

## Scope and curation rules

- **Core papers:** LLM / MLLM / speech-language models that directly perform affective representation, understanding, reasoning, generation, or emotional interaction. Vision-only/encoder-only models may be included as context but are not treated as MLLM methods.
- **Mechanism-oriented organization:** The main grouping concerns evidence modeling, model learning, and inference/interaction. Perception, reasoning, generation and interaction are **task tags**, not competing top-level branches.
- **Provenance:** `Seed` marks papers already appearing in the original literature notes; `New` marks independently identified additions. These labels **do not imply that Yali Fu has personally read or endorsed a paper**.
- **Venue accuracy:** `arXiv` means a preprint unless official acceptance is checked. For NeurIPS 2026, the official link is the conference paper-name list, not an individual paper page. Official 2026 NeurIPS status is cross-checked against the conference listing. [NeurIPS 2026](https://neurips.cc/Downloads/2026).
- **Links:** Official, arXiv, GitHub and Hugging Face are separate. An absent link is left blank rather than invented. Some benchmark papers are cross-referenced but do not count as separate research methods.
- **Study quality:** No claim of comprehensive coverage or reproducible comparisons yet. Experimental results should only be compared after confirming tasks, evaluation protocols, backbones and datasets.

## Newly identified literature: September–October 2026

Selected recent additions beyond the seed notes:

| Topic | Paper | Primary contribution |
|---|---|---|
| Frozen MLLM skill evolution | [CASE](https://arxiv.org/abs/2610.32481) | Targeted emotion-confusion skill library, training-free inference |
| Long-video affective memory | [LongEmo](https://arxiv.org/abs/2609.40079) | Event Memory Graph for long-range emotional reasoning |
| Cognitive appraisal | [CogEmo](https://arxiv.org/abs/2610.11918) | Appraisal-grounded emotion reasoning and instruction data |
| Cognitive episode tracing | [TRACE](https://arxiv.org/abs/2610.11410) | Condition–Affect–Effect reasoning and benchmark |
| Spoken empathy | [EchoChat](https://arxiv.org/abs/2610.04826) | Structured empathy reasoning with stage-aware optimization |
| Latent speech reasoning | [LoopSLM](https://arxiv.org/abs/2609.37818) | Recurrent hidden-state reasoning grounded in paralinguistic cues |
| Emotional neuron analysis | [Multilingual Emotion Neurons](https://arxiv.org/abs/2608.08772) | Neuron-level cross-language affect representation |
| Multimodal social evaluation | [SMMU](https://aclanthology.org/2026.findings-emnlp.2434/) | Long-form audio-visual social understanding, including emotion |

## Contents

- [Affective Evidence Modeling](#affective-evidence-modeling)
- [Affective Learning and Optimization](#affective-learning-and-optimization)
- [Affective Reasoning, Inference and Interaction](#affective-reasoning-inference-and-interaction)
- [Benchmarks, Datasets and Evaluation](#benchmarks-datasets-and-evaluation)
- [Related Surveys and Adjacent Work](#related-surveys-and-adjacent-work)


## Affective Evidence Modeling

- **2026 · arXiv · E2-LLM** — E^2-LLM: Bridging Neural Signals and Interpretable Affective Analysis. [arXiv](https://arxiv.org/abs/2601.07877). `New-verified`

- **2026 · arXiv · Qwen3-Omni AH Detection** — Nuanced Emotion Recognition Based on a Segment-based MLLM Framework Leveraging Qwen3-Omni for AH Detection. [arXiv](https://arxiv.org/abs/2603.13406) · [GitHub](https://github.com/dlnn123/A-H-Detection-with-Qwen-Omni). `New-verified`

- **2026 · EMNLP · UniMER** — UniMER: Multilingual Multimodal Emotion Recognition with Prototype-Guided Attention Pooling. [Official](https://aclanthology.org/2026.emnlp-main.1611/). `New-verified`

- **2026 · arXiv · FAB-G** — Attribute-Grounded Selective Reasoning for Artwork Emotion Understanding with Multimodal Large Language Models. [arXiv](https://arxiv.org/abs/2605.15755). `New-verified`

- **2026 · EMNLP · Emotion-Control Circuit** — Tracing a Sparse Emotion-Control Circuit in LLM-Based Text-to-Speech. [Official](https://aclanthology.org/2026.emnlp-main.378/) · [arXiv](https://arxiv.org/abs/2610.05080). `New-verified`

- **2024 · NeurIPS · Emotion-LLaMA** — Emotion-LLaMA: Multimodal Emotion Recognition and Reasoning with Instruction Tuning. [Official](https://proceedings.neurips.cc/paper_files/paper/2024/hash/c7f43ada17acc234f568dc66da527418-Abstract-Conference.html). `Seed`

- **2024 · EMNLP · BLSP-Emo** — BLSP-Emo: Towards Empathetic Large Speech-Language Models. [Official](https://aclanthology.org/2024.emnlp-main.1070/) · [GitHub](https://github.com/cwang621/blsp-emo). `Seed`

- **2024 · ECCV · EmoLA** — Facial Affective Behavior Analysis with Instruction Tuning. [Official](https://link.springer.com/chapter/10.1007/978-3-031-72649-1_10) · [arXiv](https://arxiv.org/abs/2404.05052). `Seed`

- **2024 · CVPR · EmoVIT** — EmoVIT: Revolutionizing Emotion Insights with Visual Instruction Tuning. [Official](https://ieeexplore.ieee.org/abstract/document/10657651) · [arXiv](https://arxiv.org/abs/2404.16670). `Seed`

- **2025 · ICML · AffectGPT** — AffectGPT: A New Dataset, Model, and Benchmark for Emotion Understanding with Multimodal Large Language Models. [Official](https://openreview.net/forum?id=xmbdACI0xu) · [arXiv](https://arxiv.org/abs/2501.16566). `Seed`

- **2025 · ICML · SEPM** — Catch Your Emotion: Sharpening Emotion Perception in Multimodal Large Language Models. [Official](https://openreview.net/forum?id=IYOksPHJKT) · [GitHub](https://github.com/fuyyyyy/SEPM). `Seed`

- **2025 · IJCV · StimuVAR** — StimuVAR: Spatiotemporal Stimuli-Aware Video Affective Reasoning with Multimodal Large Language Models. [Official](https://link.springer.com/article/10.1007/s11263-025-02495-3) · [arXiv](https://arxiv.org/abs/2409.00304) · [GitHub](https://github.com/Yuxiang-Guo/StimuVAR). `Seed`

- **2025 · ACM MM · EmoDETective** — EmoDETective: Detecting, Exploring, and Thinking Emotional Cause in Videos. [Official](https://dl.acm.org/doi/abs/10.1145/3746027.3755522) · [GitHub](https://github.com/Listever/EmoDETective). `Seed`

- **2025 · ACM MM · MoSEAR** — Benchmarking and Bridging Emotion Conflicts for Multimodal Emotion Reasoning. [Official](https://dl.acm.org/doi/abs/10.1145/3746027.3754856) · [arXiv](https://arxiv.org/abs/2508.01181) · [GitHub](https://github.com/ZhiyuanHan-Aaron/MoSEAR) · [Hugging Face](https://huggingface.co/AaronHan/MoSEAR). `Seed`

- **2025 · arXiv · Omni-Emotion** — Omni-Emotion: Extending Video MLLM with Detailed Face and Audio Modeling for Multimodal Emotion Analysis. [arXiv](https://arxiv.org/abs/2501.09502). `Seed`

- **2025 · ACM MM · FEALLM** — FEALLM: Advancing Facial Emotion Analysis in Multimodal Large Language Models with Emotional Synergy and Reasoning. [Official](https://dl.acm.org/doi/abs/10.1145/3746027.3755352) · [arXiv](https://arxiv.org/abs/2505.13419). `Seed`

- **2025 · ACM MM · EmoChat** — From Subtle Hints to Grand Expressions: Mastering Fine-grained Emotions with Dynamic Multimodal Analysis. [Official](https://dl.acm.org/doi/abs/10.1145/3746027.3754762). `Seed`

- **2026 · arXiv · Emotion-LLaMAv2** — Emotion-LLaMAv2 and MMEVerse: A New Framework and Benchmark for Multimodal Emotion Understanding. [arXiv](https://arxiv.org/abs/2601.16449) · [GitHub](https://github.com/ooochen-30/Emotion-LLaMA-v2) · [Hugging Face](https://huggingface.co/ooochen/Emotion-LLaMA-v2). `Seed`

- **2026 · arXiv · UniFER** — Rethinking Facial Expression Recognition in the Era of Multimodal Large Language Models: Benchmark, Datasets, and Beyond. [arXiv](https://arxiv.org/abs/2511.00389) · [GitHub](https://github.com/zfkarl/UniFER) · [Hugging Face](https://huggingface.co/Karl28/UniFER-7B). `Seed`

- **2026 · ACL Findings · EmoMM** — EmoMM: Benchmarking and Steering MLLM for Multimodal Emotion Recognition under Conflict and Missingness. [Official](https://aclanthology.org/2026.findings-acl.1018/) · [arXiv](https://arxiv.org/abs/2605.01024). `Seed`

- **2026 · arXiv · Multilingual Emotion Neurons** — Multilingual Emotion Neurons in Large Audio-Language Models. [arXiv](https://arxiv.org/abs/2608.08772). `New`

- **2026 · arXiv · Emotion Concepts** — Do Emotion Concepts Generalize Across Sources, Modalities, and Architectures in Vision-Language Models?. [arXiv](https://arxiv.org/abs/2609.34742). `New`

- **2026 · arXiv · PI-MLLM** — PI-MLLM: Psychophysics-Inspired Multimodal Large Language Model for Oddly Satisfying Video Emotion Analysis. [arXiv](https://arxiv.org/abs/2610.28264). `New`

- **2026 · arXiv · Brain-Aligned MLLMs** — Brain-Aligned Multimodal LLMs for Social and Emotional Understanding of Cartoon Movies. [arXiv](https://arxiv.org/abs/2610.22706). `New`

## Affective Learning and Optimization

- **2026 · EMNLP Findings · SoVTR** — SoVTR: Set-of-Vision-Text Rewards for Attribute-Grounded Emotion Recognition in VLLMs. [Official](https://aclanthology.org/2026.findings-emnlp.1807/). `New-verified`

- **2026 · ICLR · TMPO** — Unveiling the Cognitive Compass: Theory-of-Mind-Guided Multimodal Emotion Reasoning. [Official](https://proceedings.iclr.cc/paper_files/paper/2026/hash/89ab43b626b480347dbaccda7be8aedb-Abstract-Conference.html) · [arXiv](https://arxiv.org/abs/2602.00971). `New-verified`

- **2025 · arXiv · R1-Omni** — R1-Omni: Explainable Omni-Multimodal Emotion Recognition with Reinforcement Learning. [arXiv](https://arxiv.org/abs/2503.05379). `Seed`

- **2025 · arXiv · AffectGPT-R1** — AffectGPT-R1: Leveraging Reinforcement Learning for Open-Vocabulary Multimodal Emotion Recognition. [arXiv](https://arxiv.org/abs/2508.01318). `Seed`

- **2025 · ACM MM · M3F** — Emotion across Modalities and Cultures: Multilingual Multimodal Emotion-Cause Analysis with Memory-inspired Framework. [Official](https://dl.acm.org/doi/abs/10.1145/3746027.3755655). `Seed`

- **2026 · CVPR · EMO-R3** — EMO-R3: Reflective Reinforcement Learning for Emotional Reasoning in Multimodal Large Language Models. [Official](https://openaccess.thecvf.com/content/CVPR2026/html/Fang_EMO-R3_Reflective_Reinforcement_Learning_for_Emotional_Reasoning_in_Multimodal_Large_CVPR_2026_paper.html) · [arXiv](https://arxiv.org/abs/2602.23802). `Seed`

- **2026 · AAAI · Facial-R1** — Facial-R1: Aligning Reasoning and Recognition for Facial Emotion Analysis. [Official](https://ojs.aaai.org/index.php/AAAI/article/view/39906) · [arXiv](https://arxiv.org/abs/2511.10254) · [GitHub](https://github.com/RobitsG/Facial-R1). `Seed`

- **2026 · ACL Findings · CAIR** — CAIR: Causal Adaptive Information-based Reinforcement Learning for Multimodal Emotion Reasoning. [Official](https://aclanthology.org/2026.findings-acl.1263/). `Seed`

- **2026 · ICML · OPPO** — Omni-Perception Policy Optimization for Multimodal Emotion Reasoning. [Official](https://openreview.net/forum?id=4dwe2wlxx5) · [arXiv](https://arxiv.org/abs/2606.25325) · [GitHub](https://github.com/ZhiyuanHan-Aaron/OPPO) · [Hugging Face](https://huggingface.co/AaronHan/OPPO). `Seed`

- **2026 · arXiv · OmniOPSD** — OmniOPSD: Rationale-Privileged On-Policy Self-Distillation for Affective Computing. [arXiv](https://arxiv.org/abs/2606.15920) · [GitHub](https://github.com/ZebangCheng/OmniOPSD). `Seed`

- **2026 · NeurIPS · AffectGPT-RL** — AffectGPT-RL: Revealing Roles of Reinforcement Learning in Open-Vocabulary Emotion Recognition. [Official](https://neurips.cc/Downloads/2026) · [arXiv](https://arxiv.org/abs/2605.06126) · [GitHub](https://github.com/zeroQiaoba/AffectGPT/tree/master/AffectGPT-RL). `Seed`

- **2026 · arXiv · Light-MER** — Do We Really Need Multimodal Emotion Language Models Larger Than 1B Parameters?. [arXiv](https://arxiv.org/abs/2607.12787) · [GitHub](https://github.com/GAIR-Lab/Light-MER). `Seed`

- **2026 · arXiv · OneEmo** — OneEmo: A Unified Multimodal Reasoning Model for Emotion Perception, Understanding, and Interaction. [arXiv](https://arxiv.org/abs/2608.06013). `Seed`

- **2026 · arXiv · CogEmo** — From Surface to Depth: Towards Cognitive Appraisal Reasoning in Multimodal Emotion Understanding. [arXiv](https://arxiv.org/abs/2610.11918) · [GitHub](https://github.com/MSA-LMC/CogEmo). `New`

- **2026 · arXiv · TRACE** — Cognition-Oriented Emotion Tracing from Causes to Consequences in Real-World Social Scenes. [Official](https://cogaffc.github.io/TRACE) · [arXiv](https://arxiv.org/abs/2610.11410). `New`

- **2026 · Pattern Recognition · EMARF** — Unlocking Explainable and Effective Multimodal Affective Reasoning via Large Language Models. [Official](https://www.sciencedirect.com/science/article/pii/S0031320326003316). `New`

## Affective Reasoning, Inference and Interaction

- **2026 · arXiv · HMER** — Multi-Faceted Evaluation and Mitigation of Emotion Hallucinations in MLLMs. [arXiv](https://arxiv.org/abs/2609.11154). `New-verified`

- **2026 · EMNLP · TRACE-Streaming** — Emotion Understanding in Streaming Video with Trajectory-Aware Reliability. [Official](https://aclanthology.org/2026.emnlp-main.554/). `New-verified`

- **2024 · EMNLP · AlignCap** — Aligning Speech Emotion Captioning to Human Preferences. [Official](https://aclanthology.org/2024.emnlp-main.224/) · [arXiv](https://arxiv.org/abs/2410.19134). `Seed`

- **2024 · AAAI · SECap** — SECap: Speech Emotion Captioning with Large Language Model. [Official](https://ojs.aaai.org/index.php/AAAI/article/view/29902) · [GitHub](https://github.com/thuhcsi/SECap). `Seed`

- **2025 · EMNLP · MERMAID** — MERMAID: Multi-perspective Self-reflective Agents with Generative Augmentation for Emotion Recognition. [Official](https://aclanthology.org/2025.emnlp-main.1252/). `Seed`

- **2025 · ACM MM · Agent-MER** — A Cognitive Agent with Hierarchical Deliberation for Open-Vocabulary Multimodal Emotion Recognition. [Official](https://dl.acm.org/doi/abs/10.1145/3746027.3762011). `Seed`

- **2025 · ACM MM · Affective-CoT** — Affective-CoT: Decomposing Multimodal Emotion Reasoning through a Hierarchical Cognitive Workflow. [Official](https://dl.acm.org/doi/abs/10.1145/3746027.3762009) · [GitHub](https://github.com/GPNU-AIoT/Affective-CoT). `Seed`

- **2025 · EMNLP Findings · FIRES** — Flexible Thinking for Multimodal Emotional Support Conversation via Reinforcement Learning. [Official](https://aclanthology.org/2025.findings-emnlp.70/). `Seed`

- **2026 · AAAI · ERV** — Emotion-Coherent Reasoning for Multimodal LLMs via Emotional Rationale Verifier. [Official](https://ojs.aaai.org/index.php/AAAI/article/view/37184) · [arXiv](https://arxiv.org/abs/2510.23506) · [GitHub](https://github.com/Rhatanii/ERV). `Seed`

- **2026 · ICMR · CERA** — CERA: Conflict-Explicit Reflective Agent for Multimodal Emotion Reasoning. [Official](https://dl.acm.org/doi/abs/10.1145/3805622.3810634). `Seed`

- **2026 · arXiv · AffectAgent** — AffectAgent: Collaborative Multi-Agent Reasoning for Retrieval-Augmented Multimodal Emotion Recognition. [arXiv](https://arxiv.org/abs/2604.12735) · [GitHub](https://github.com/Wz1h1NG/AffectAgent). `Seed`

- **2026 · SIGIR · GraphEMO** — A Graph-Enhanced MLLM for Hierarchical Multimodal Emotion Understanding and Support in Conversations. [Official](https://dl.acm.org/doi/abs/10.1145/3805712.3809910). `Seed`

- **2026 · arXiv · EmoOmni** — EmoOmni: Bridging Emotional Understanding and Expression in Omni-Modal LLMs. [arXiv](https://arxiv.org/abs/2602.21900). `Seed`

- **2026 · arXiv · MER-R1** — MER-R1: Multimodal Emotion Reasoning via Slow-Fast Thinking Synergy. [arXiv](https://arxiv.org/abs/2606.27652). `Seed`

- **2026 · arXiv · LongEmo** — LongEmo: Towards Emotion Understanding and Reasoning in Long Videos. [arXiv](https://arxiv.org/abs/2609.40079). `New`

- **2026 · arXiv · Affective Nuances** — Decoding Affective Nuances: Enhancing MLLMs via Hierarchical Emotion Reasoning and Contrastive Discriminative Pruning. [arXiv](https://arxiv.org/abs/2609.36782). `New`

- **2026 · arXiv · CASE** — CASE: Confusion-Aware Skill Evolution for Frozen Multimodal Emotion Models. [arXiv](https://arxiv.org/abs/2610.32481). `New`

- **2026 · NeurIPS · EchoChat / EmpathyChat** — EchoChat: Structured Cognitive Reasoning in Empathetic Spoken Dialogue. [NeurIPS 2026 paper list](https://neurips.cc/Downloads/2026) · [arXiv](https://arxiv.org/abs/2610.04826) · [GitHub](https://github.com/dingdongwang/EchoChat). `New` · *The NeurIPS index currently uses the title **EmpathyChat**; the authors' homepage and arXiv use **EchoChat**. Treated as one work pending final proceedings metadata.*

- **2026 · arXiv · LoopSLM** — Thinking in Depth, Speaking Directly: Recurrent Latent Reasoning for Paralinguistically Grounded Spoken Dialogue. [arXiv](https://arxiv.org/abs/2609.37818). `New`

## Benchmarks, Datasets and Evaluation

- **2026 · ACL · EmoS** — EmoS: A High-Fidelity Multimodal Benchmark for Fine-grained Streaming Emotional Understanding. [Official](https://aclanthology.org/2026.acl-long.1813/) · [GitHub](https://github.com/NLP2CT/EmoS). `New-verified`

- **2026 · EMNLP · MER-Bench** — MER-Bench: Benchmarking Multimodal Emotional Reappraisal for Image-Text Memes. [Official](https://aclanthology.org/2026.emnlp-main.940/). `New-verified`

- **2026 · EMNLP Findings · CREMA-ASIS** — When Vocal Tone and Literal Meaning Diverge: An Acoustic–Semantic Incongruity Study for Large Audio–Language Models. [Official](https://aclanthology.org/2026.findings-emnlp.35/). `New-verified`

- **2026 · EMNLP · SEA-SpeechBench** — SEA-SpeechBench: A Large-Scale Multitask Benchmark for Speech Understanding Across Southeast Asia. [Official](https://aclanthology.org/2026.emnlp-main.1934/). `New-verified`

- **2026 · EMNLP · ToM-Video** — ToM-Video: A Theory-of-Mind Video Benchmark with Spatio-Temporal Grounded Reasoning. [Official](https://aclanthology.org/2026.emnlp-main.302/). `New-verified`

- **2023 · ACM MM · MER 2023** — MER 2023: Multi-label Learning, Modality Robustness, and Semi-Supervised Learning. [Official](https://dl.acm.org/doi/abs/10.1145/3581783.3612836) · [arXiv](https://arxiv.org/abs/2304.08981). `Seed`

- **2024 · ACM Workshop · MER 2024** — MER 2024: Semi-Supervised Learning, Noise Robustness, and Open-Vocabulary Multimodal Emotion Recognition. [Official](https://dl.acm.org/doi/abs/10.1145/3689092.3689959) · [arXiv](https://arxiv.org/abs/2404.17113) · [GitHub](https://github.com/zeroQiaoba/MERTools/tree/master/MER2024). `Seed`

- **2025 · ACM MM · MER 2025** — MER 2025: When Affective Computing Meets Large Language Model. [Official](https://dl.acm.org/doi/abs/10.1145/3746027.3762007) · [arXiv](https://arxiv.org/abs/2504.19423) · [GitHub](https://github.com/zeroQiaoba/MERTools) · [Hugging Face](https://huggingface.co/datasets/MERChallenge/MER2025). `Seed`

- **2025 · ACM MM · CA-MER** — Benchmarking and Bridging Emotion Conflicts for Multimodal Emotion Reasoning. [Official](https://dl.acm.org/doi/abs/10.1145/3746027.3754856) · [arXiv](https://arxiv.org/abs/2508.01181) · [GitHub](https://github.com/ZhiyuanHan-Aaron/MoSEAR). `Seed-cross-reference`

- **2026 · arXiv · MER 2026** — MER 2026: From Discriminative Emotion Recognition to Generative Emotion Understanding. [Official](https://zeroqiaoba.github.io/MER-Challenge/) · [arXiv](https://arxiv.org/abs/2604.19417). `Seed`

- **2026 · ICLR · MME-Emotion** — MME-Emotion: A Holistic Evaluation Benchmark for Emotional Intelligence in Multimodal Large Language Models. [Official](https://proceedings.iclr.cc/paper_files/paper/2026/hash/50d277e84b2bcbaadcd84548a87e8cc4-Abstract-Conference.html) · [arXiv](https://arxiv.org/abs/2508.09210) · [GitHub](https://github.com/QwenAudio/MME-Emotion) · [Hugging Face](https://huggingface.co/datasets/Karl28/MME-Emotion). `Seed`

- **2026 · ICLR · EmotionHallucer** — EmotionHallucer: Evaluating Emotion Hallucinations in Multimodal Large Language Models. [Official](https://proceedings.iclr.cc/paper_files/paper/2026/hash/a80546907c520409ce3c0e226c1f7e5f-Abstract-Conference.html) · [arXiv](https://arxiv.org/abs/2505.11405) · [GitHub](https://github.com/xxtars/EmotionHallucer). `Seed`

- **2026 · ICLR · MVEI** — Customizing Visual Emotion Evaluation for MLLMs: An Open-vocabulary, Multifaceted, and Scalable Approach. [arXiv](https://arxiv.org/abs/2509.21950). `Seed`

- **2026 · arXiv · ESE** — Watching Movies Like a Human: Egocentric Emotion Understanding for Embodied Companions. [arXiv](https://arxiv.org/abs/2604.15823). `Seed`

- **2026 · arXiv · FERBENCH** — Rethinking Facial Expression Recognition in the Era of Multimodal Large Language Models: Benchmark, Datasets, and Beyond. [arXiv](https://arxiv.org/abs/2511.00389) · [GitHub](https://github.com/zfkarl/UniFER) · [Hugging Face](https://huggingface.co/datasets/Karl28/UniFER). `Seed-cross-reference`

- **2026 · ECCV · DAR** — Benchmarking Dynamic Affective Reasoning: A Viewer-Centric Video Emotion Dataset. [arXiv](https://arxiv.org/abs/2607.10238) · [GitHub](https://github.com/Zhang-Zhiyan/DAR) · [Hugging Face](https://huggingface.co/datasets/aiaiaizzy/DAR-R1). `Seed`

- **2026 · arXiv · EmoTrans** — EmoTrans: A Benchmark for Understanding, Reasoning, and Predicting Emotion Transitions in Multimodal LLMs. [arXiv](https://arxiv.org/abs/2604.23348). `Seed`

- **2026 · arXiv · EmoBench-M** — EmoBench-M: Benchmarking Emotional Intelligence for Multimodal Large Language Models. [arXiv](https://arxiv.org/abs/2502.04424). `Seed`

- **2026 · ECCV · SpEmoC** — SpEmoC: A Balanced Speaker-Segment Multimodal Emotion Benchmark. [Official](https://skvipparthi.com/spemoc.html) · [arXiv](https://arxiv.org/abs/2607.18109) · [GitHub](https://github.com/saniajmi/SpEmoC-ECCV2026). `Seed`

- **2026 · NeurIPS · CAREBench** — CAREBench: Evaluating LLMs' Emotion Understanding by Assessing Cognitive Appraisal Reasoning. [Official](https://neurips.cc/Downloads/2026) · [arXiv](https://arxiv.org/abs/2605.17176). `New-adjacent-text`

- **2026 · EMNLP · Emotion Experience/Expression/Perception** — Emotion Experience, Expression, and Perception: Emotion Analysis on Multimodal Social Media Posts. [Official](https://aclanthology.org/2026.emnlp-main.306/) · [arXiv](https://arxiv.org/abs/2609.18385). `New`

- **2026 · EMNLP Findings · SMMU** — SMMU: Benchmarking Social Intelligence of Multimodal Large Language Models. [Official](https://aclanthology.org/2026.findings-emnlp.2434/). `New-adjacent-social`

## Related Surveys and Adjacent Work

- **2026 · EMNLP · EmoDap** — EmoDap: Dual-Agent Prompt Retrieval Framework for Zero-Shot Fine-Grained Emotion Recognition. [Official](https://aclanthology.org/2026.emnlp-main.1167/). `New-verified`

- **2026 · EMNLP Findings · EIBench** — EIBench: A Simulator-Based Benchmark and Turn-Credit RL for Emotion Management. [Official](https://aclanthology.org/2026.findings-emnlp.789/). `New-verified`

- **2026 · EMNLP · EmoLASP** — EmoLASP: Emotion Recognition with Language Models and Answer Set Programming. [Official](https://aclanthology.org/2026.emnlp-main.1769/). `New-verified`

- **2026 · EMNLP Findings · Layer-wise Emotion Probing** — Some Emotions Run Deeper: Layer-wise Probing and Causal Intervention in Large Language Models. [Official](https://aclanthology.org/2026.findings-emnlp.421/). `New-verified`

- **2026 · EMNLP · Sparse Emotion Features** — Why Are Some Emotions Harder for LLMs? Uncovering the Causal Mechanisms of Emotion Inference via Sparse Autoencoders. [Official](https://aclanthology.org/2026.emnlp-main.559/). `New-verified`

- **2026 · EACL Findings · AHaBench** — Being Kind Isn’t Always Being Safe: Diagnosing Affective Hallucination in LLMs. [Official](https://aclanthology.org/2026.findings-eacl.4/) · [GitHub](https://github.com/anonymous9268/AHaBench). `New-verified`

- **2026 · IJCAI · MER+LLMs Survey** — Multimodal Emotion Recognition with Large Language Models. [Official](https://ijcai.org/proceedings/2026/897) · [arXiv](https://arxiv.org/abs/2605.21239). `Seed`

- **2025 · arXiv · MER+Reasoning Survey** — Multimodal Large Language Models Meet Multimodal Emotion Recognition and Reasoning: A Survey. [arXiv](https://arxiv.org/abs/2509.24322). `Seed`

- **2026 · KBS · NLP Affective Survey** — Affective Computing in the Era of Large Language Models: A Survey from the NLP Perspective. [arXiv](https://arxiv.org/abs/2408.04638). `Seed`

- **2025 · EMNLP Findings · MERC Survey** — Multimodal Emotion Recognition in Conversations: A Survey of Methods, Trends, Challenges and Prospects. [Official](https://aclanthology.org/2025.findings-emnlp.332.pdf) · [arXiv](https://arxiv.org/abs/2505.20511). `Seed`

- **2026 · Applied Sciences · Unified Affective AI Survey** — Towards Unified Affective AI: A Cross-Modal Survey of Emotion Recognition, Generation, and Control. [Official](https://www.mdpi.com/2076-3417/16/18/9333). `New`

- **2026 · NeurIPS · Affective AI Safety** — Affective AI Safety: The Missing Piece in LLM Safety. [Official](https://neurips.cc/Downloads/2026) · [arXiv](https://arxiv.org/abs/2606.23380). `New-adjacent-position`

- **2026 · EMNLP · Why It Hurts** — Why It Hurts: Identifying the Drivers of Negative Thoughts in Emotional Support Conversations. [Official](https://aclanthology.org/2026.emnlp-main.722/) · [arXiv](https://arxiv.org/abs/2607.28648). `New-adjacent-text`

## Inclusion and extraction checklist

For each newly added paper, record: **publication status**, date, input/output modalities, target affective task, main contribution, training paradigm, backbone, public code and dataset, evaluation protocol, and whether the paper uses generative MLLM inference. For method papers, assign one *primary* method category with cross-references for secondary mechanisms.

**Recommended comparisons:** (1) feature alignment vs. explicit emotion-grounded evidence; (2) SFT vs. RL vs. training-free adaptation; (3) final-answer rewards vs. evidence/rationale rewards; (4) prompt/agent/memory/retrieval-based inference; (5) expressed vs. perceived vs. evoked emotions and personalization.

**Coverage:** 94 README listings representing **92 unique papers** after merging the two explicit method/benchmark cross-references (MoSEAR/CA-MER and UniFER/FERBENCH) (including 18 independently identified and official/arXiv-verified papers in this update; earlier `New` records remain). Some benchmark entries are explicit cross-references and must not be counted as separate unique papers. Snapshot: 2026-10-29. Maintainer: Yali Fu.

