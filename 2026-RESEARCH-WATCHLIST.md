# 2026 Research Watchlist: Recent Affective MLLM Work

Updated: **2026-10-29** · Curated for research planning by **Yali Fu**.

**Status labels:** `Conference` = an available official conference listing or verified author/publication record; `Preprint` = arXiv without separately verified venue. `Adjacent` denotes work that is not a core multimodal affective method.

## Recent methodological advances

| Publication status | Paper | What the work contributes | Suggested survey lens |
|---|---|---|---|
| NeurIPS 2026 | [AffectGPT-RL](https://arxiv.org/abs/2605.06126) | Studies how reinforcement learning changes open-vocabulary affect recognition | Learning signal and reward design |
| NeurIPS 2026; title variant | [EchoChat / EmpathyChat](https://arxiv.org/abs/2610.04826) | Speech-grounded, step-structured empathetic reasoning and optimization | Speech alignment; process-level RL |
| Preprint, Oct 2026 | [CASE](https://arxiv.org/abs/2610.32481) | Emotion-pair expertise as reusable skills while freezing the MLLM | Training-free affective skill adaptation |
| Preprint, Sep 2026 | [LongEmo](https://arxiv.org/abs/2609.40079) | Memory graph for emotion reasoning across long-video events | Episodic memory and temporal inference |
| Preprint, Oct 2026 | [CogEmo](https://arxiv.org/abs/2610.11918) | Appraisal-grounded emotion understanding and instruction-tuning data | Beyond superficial cue-to-label shortcuts |
| Preprint, Oct 2026 | [TRACE](https://arxiv.org/abs/2610.11410) | Condition–Affect–Effect benchmark and structured cognitive reasoning | Emotion causes, regulation and consequences |
| Preprint, Sep 2026 | [LoopSLM](https://arxiv.org/abs/2609.37818) | Recurrent latent reasoning for empathetic spoken dialogue | Efficient paralinguistic reasoning |
| Preprint, Aug 2026 | [Multilingual Emotion Neurons](https://arxiv.org/abs/2608.08772) | Causal neuron-level emotion probes across speech languages | Internal affect representation |
| Preprint, Oct 2026 | [Brain-Aligned MLLMs](https://arxiv.org/abs/2610.22706) | Compares temporal affect/ToM judgments with human and fMRI signals | External validity and neuro-alignment |

## Evaluation and adjacent research

| Publication status | Paper | Why it matters |
|---|---|---|
| NeurIPS 2026 (adjacent; text LLM) | [CAREBench](https://arxiv.org/abs/2605.17176) | Cognitive appraisal instead of flat emotion labeling |
| EMNLP 2026 | [Emotion Experience, Expression, and Perception](https://aclanthology.org/2026.emnlp-main.306/) | Distinguishes multiple affective targets in social posts |
| EMNLP Findings 2026 (adjacent social intelligence) | [SMMU](https://aclanthology.org/2026.findings-emnlp.2434/) | Long-form audio-visual social reasoning with an emotion dimension |
| 2026 Pattern Recognition | [EMARF](https://www.sciencedirect.com/science/article/pii/S0031320326003316) | Combines MLLM extraction, consistency-guided reasoning and LoRA |
| 2026 Applied Sciences (survey) | [Towards Unified Affective AI](https://www.mdpi.com/2076-3417/16/18/9333) | Broad emotion recognition/generation/control survey; important for positioning |

## Survey questions prompted by these papers

1. **Affective grounding:** Do improvements originate from emotion-specific representations, better visual/audio evidence retrieval, or label-prior exploitation?
2. **RL objectives:** Which learning signals optimize outcome accuracy, faithful evidence grounding, calibrated uncertainty, or response appropriateness?
3. **Reasoning vs. surface cues:** How do cognitive appraisal, causal tracing, and counterfactual testing demonstrate reasoning rather than emotion-language pattern matching?
4. **Long-horizon and personalized affect:** Are episodic memory and individual preferences explicitly modeled, and do the benchmarks genuinely test them?
5. **Unified evaluation:** How should recognition, causal reasoning, emotion understanding, expressed/evoked emotion and empathetic interaction be assessed without mixing incompatible metrics?

## Metadata caution

The NeurIPS 2026 indexed paper title **EmpathyChat: Structured Cognitive Reasoning in Empathetic Spoken Dialogue** corresponds to author/arXiv **EchoChat: Structured Cognitive Reasoning in Empathetic Spoken Dialogue** (same project/authors). They are **one paper**, not two separate works. Before submission, use the published proceedings' final citation title. [NeurIPS 2026 paper index](https://neurips.cc/Downloads/2026) · [Author homepage](https://dingdongwang.github.io/).

This watchlist is a research prioritization aid, not a guarantee of complete 2026 coverage or that each paper has been read in full.
