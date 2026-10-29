# Benchmark Coverage and Evaluation Protocols for Affective MLLMs

**Snapshot: 2026-10-29** · This file records *what a dataset intends to evaluate*, not a ranking or verified performance table. Source links are official conference pages or arXiv author abstracts; counts and metrics not independently confirmed in full papers are intentionally omitted.

## 1. Capability-specific benchmark matrix

| Benchmark / paper | Evaluation target | Main affective setting | Special test condition | Publication |
|---|---|---|---|---|
| [MER-UniBench / AffectGPT](https://openreview.net/forum?id=xmbdACI0xu) | Open-vocabulary emotion understanding | Multimodal emotion labels / descriptions | General MLLM emotion understanding | ICML 2025 |
| [MER 2023](https://arxiv.org/abs/2304.08981) | Emotion recognition | Video, audio and text | Multilabel / robustness / semi-supervised | ACM MM 2023 |
| [MER 2025](https://arxiv.org/abs/2504.19423) | Emotion recognition with language models | Multimodal emotion reasoning and descriptions | Modern LLM-based evaluation | ACM MM 2025 |
| [MER 2026](https://arxiv.org/abs/2604.19417) | Generative emotion understanding | Audio, video, text and physiological signals | Generative vs discriminative | arXiv 2026 |
| [CA-MER / MoSEAR](https://arxiv.org/abs/2508.01181) | Robust emotion recognition under conflict | Conflicting audio/video/text emotion cues | Video-aligned, audio-aligned, consistent subsets | ACM MM 2025 |
| [EmoMM / CHASE](https://aclanthology.org/2026.findings-acl.1018/) | Recognition under conflicting/missing evidence | Audio, video and text | Evidence omission and modality preference | ACL Findings 2026 |
| [EmotionHallucer](https://proceedings.iclr.cc/paper_files/paper/2026/hash/a80546907c520409ce3c0e226c1f7e5f-Abstract-Conference.html) | Emotion hallucination detection | Psychology knowledge and multimodal perception | Adversarial binary QA | ICLR 2026 |
| [HMER / EHR](https://arxiv.org/abs/2609.11154) | Faceted emotion hallucination measurement | Generative multimodal emotion rationales | Expression/action/audio; instinct/logic/conclusion facets | arXiv 2026 |
| [MME-Emotion](https://proceedings.iclr.cc/paper_files/paper/2026/hash/50d277e84b2bcbaadcd84548a87e8cc4-Abstract-Conference.html) | Multimodal emotional understanding and reasoning | Audio-visual affect | Cross-scenario reasoning/generalization | ICLR 2026 |
| [EMER-CoT / GEM](https://doi.org/10.1109/TAFFC.2026.3713090) | Cue--cause--emotion explanation structure | Vision, audio and text affective rationales | Graph-based cue coverage, relation reconstruction and emotion consistency | IEEE T-AFFC 2026; linked to EMO-CoT | 
| [CogEmo-Bench](https://arxiv.org/abs/2610.11918) | Appraisal-grounded emotional reasoning | Event appraisal across six dimensions | Appraisal Evidence Quality Score | arXiv 2026 |
| [HitEmotion / TMPO](https://proceedings.iclr.cc/paper_files/paper/2026/hash/89ab43b626b480347dbaccda7be8aedb-Abstract-Conference.html) | Theory-of-Mind-grounded affective reasoning | Multimodal social/mental states | Increasing cognitive-depth requirements | ICLR 2026 |
| [DAR](https://arxiv.org/abs/2607.10238) | Dynamic, viewer-centric emotion reasoning | Video emotion | Viewer subjectivity, temporal evolution | ECCV 2026 |
| [EmoTrans](https://arxiv.org/abs/2604.23348) | Emotion transition prediction | Audio/video/text | Emotion shifts over time | arXiv 2026 |
| [LongEmoBench](https://arxiv.org/abs/2609.40079) | Long-video emotion reasoning | Multi-event video narratives | Episodic long-horizon memory dependency | arXiv 2026 |
| [EmoS](https://aclanthology.org/2026.acl-long.1813/) | Streaming fine-grained emotional understanding | Monologues and continuous signals | Static slices versus streaming prefixes | ACL 2026 |
| [MER-Bench](https://aclanthology.org/2026.emnlp-main.940/) | Emotional reappraisal and multimodal generation | Image-text memes | Affective editing + embedded text preservation | EMNLP 2026 |
| [CREMA-ASIS](https://aclanthology.org/2026.findings-emnlp.35/) | Audio-language emotion/sentiment incongruity | Speech tone and semantic sentiment | Acoustic vs semantic conflicts | EMNLP Findings 2026 |
| [SEA-SpeechBench](https://aclanthology.org/2026.emnlp-main.1934/) | General multilingual speech model abilities **(adjacent)** | Speech processing, emotion and temporal tasks | 11 SEA languages; emotion is only one dimension | EMNLP 2026 |
| [SMMU](https://aclanthology.org/2026.findings-emnlp.2434/) | Social intelligence **(adjacent)** | Long-form audiovisual scenes | Emotion + intent, beliefs, perspectives and relations | EMNLP Findings 2026 |
| [AHaBench](https://aclanthology.org/2026.findings-eacl.4/) | Affective hallucination and social dependency **(text-only adjacent)** | Emotionally vulnerable advice dialogue | Enmeshment, presence illusion, overdependence | EACL Findings 2026 |
| [EIBench](https://aclanthology.org/2026.findings-emnlp.789/) | Multi-turn emotion management **(text-only adjacent)** | Interactive simulated dialogues | Support, Defense, Repair, Charm; turn-level credit | EMNLP Findings 2026 |

**Cross-reference rule:** Benchmark/method pairs such as *MoSEAR/CA-MER*, *UniFER/FERBENCH*, *CogEmo/CogEmo-Bench* and *LongEmo/LongEmoBench* are not independent papers unless the dataset has its own separate publication. Use the canonical paper table in [papers.csv](papers.csv).

## 2. Evaluation dimensions that must be distinguished

| Dimension | What it evaluates | Critical error if pooled |
|---|---|---|
| Closed-set emotion recognition | Category prediction for predefined taxonomy | Treating accuracy/F1 as evidence of free-form reasoning |
| Open-vocabulary emotion recognition | Descriptive emotion outputs | Scoring as if fixed labels were predicted |
| Emotion cause / cognitive appraisal | Causal or mental-state evidence behind affect | Confusing fluent narratives with faithful evidence |
| Subjective evoked emotion | Viewer/reader reaction to content | Conflating depicted actor emotion with audience emotion |
| Emotional speech expression | Audible expression conditioned on intended tone | Treating ASR accuracy as prosody quality |
| Empathetic response appropriateness | Context-sensitive interpersonal response | Equating positive sentiment with useful support |
| Multi-turn emotion management | State or relational effect across dialogue | Evaluating only a single-turn response |
| Emotion hallucination | Unsupported perceptual or mental-state assertions | Merging all error types into factual QA hallucination |
| Robustness | Missing, corrupted or conflicting modalities | Reporting only clean benchmark scores |
| Cross-person / cross-cultural shifts | Adaptation across speakers, cultures, domains | Treating in-distribution gains as out-of-distribution competence |

## 3. Minimal protocol fields before reporting a SOTA table

For every row, verify in the original paper:

1. Dataset version, exact split and whether benchmark authors release labels.
2. Input modality and available context (video length, speech, text transcript, physiological signals).
3. Training data leakage / overlap and in-domain vs cross-domain setting.
4. MLLM backbone size, encoder components, LoRA/full training and inference-time external models.
5. Prompt, number of samples, LLM judge, judge prompts/version and human rater protocol.
6. Metrics: classification F1/accuracy, rubric scores, generation scores, user state improvement, reliability and safety; report scales and direction.
7. Whether results are directly reproduced, copied from paper, or estimated. Never imply a new experiment was conducted.

## 4. Proposed analysis figures for the survey

- **Benchmark coverage heatmap:** rows = datasets, columns = Perception / Appraisal / Reasoning / Generation / Interaction / Reliability; mark *covered*, *partially covered*, *not evaluated* only after reading the evaluation section.
- **Modality coverage matrix:** Text, Image, Video, Audio, Physiological; distinguish explicit native model input from human/LLM-generated textual descriptions of that modality.
- **Evaluation validity map:** expressed / perceived / evoked / experienced emotion; annotation subject; temporal window; identity/scene shift.
- **Performance comparisons:** split into distinct task-specific tables, never combine all affective tasks into one composite SOTA ranking without a transparent common evaluator.

## 5. Immediate reading priorities

**Evidence faithfulness:** EmotionHallucer, HMER/EHR, SoVTR, TMPO, CogEmo.  
**Temporal and interactive emotion:** LongEmoBench, EmoS, EmoTrans, DAR, EIBench (text-only reference).  
**Multimodal reliability:** CA-MER, EmoMM, CREMA-ASIS, UniMER (cross-lingual).  
**Expression and generation:** MER-Bench, EmoOmni; add more speech and emotional generation benchmarks before finalizing Section 5.

*This is an audit-oriented mapping, not a systematic review or literature-quality ranking.*
