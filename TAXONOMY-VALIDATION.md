# Taxonomy Validation and Survey Evidence Matrix

**Survey:** *Affective Intelligence in Multimodal Large Language Models: A Comprehensive Survey*  
**Research snapshot:** 2026-10-29 · **Status:** provisional, abstract-level validation; full-paper review pending  
**Companion catalog:** [README](README.md) · [Canonical records](papers.csv)

## 1. Methodological principle

The survey should **not** merely reuse the Perception → Reasoning → Generation capability sequence as its method taxonomy. Existing surveys already cover recognition and reasoning, and affective computing work routinely spans several capabilities. Instead, organize the main method chapters around the **primary locus of technical intervention**:

| Main section | Intervention locus | Main technical question | Typical components |
|---|---|---|---|
| **Affective Evidence Modeling** | Representations, sensory evidence, cross-modal links and grounding | What affective cues are extracted and how are they reconciled? | modality encoders, projection/alignment, evidence selection, temporal grounding, conflict handling |
| **Affective Learning and Optimization** | Training objective, feedback, parameter updates | Which data or learning signals establish affective competence? | affective SFT, contrastive/prototype learning, outcome/process RL, preference optimization, self-distillation |
| **Affective Reasoning, Inference and Interaction** | Runtime computation and response policy | How does the system select, verify, remember and act on affective evidence? | structured prompting, deliberation, verification, memory/RAG, skill reuse, emotional speech/dialogue |

The **secondary axis** is the affective *capability* (Perception, Understanding, Reasoning, Generation, Interaction). These two axes must not be treated as independent empirical observations until the full papers and evaluations are read.

**Assignment rule:** Put a method where the principal novelty is established. A method may also be tagged under its task outcomes, but should not be reviewed at full length in several sections. For benchmarks, use a separate evaluation section.

### Important boundary cases

- **SoVTR:** The face/body/context evidence is essential, but its *central intervention* is reward design and GRPO; primary chapter = Learning.
- **HMER:** Evaluates hallucination and uses two memories to rectify unreliable affective reasoning; primary chapter = Inference, benchmark discussed briefly in Evaluation.
- **CogEmo:** Combines appraisal instruction data, sparse MoE adaptation and a benchmark. Primary placement depends on a full-paper inspection of its principal contribution; do not infer from the word “Reasoning” alone.
- **EmoOmni:** A trained generative architecture does not become an “inference-time method” simply because it emits speech. Its architectural/training aspects must be explicitly distinguished from its response policy.
- **Two TRACE methods:** [Cognition-oriented TRACE (Oct arXiv)](https://arxiv.org/abs/2610.11410) and [TRACE-Streaming (EMNLP)](https://aclanthology.org/2026.emnlp-main.554/) are **different papers** with overlapping acronyms.

## 2. Representative paper-to-mechanism mapping

The following mechanism descriptions are derived from **public abstracts** and official venue descriptions, not a claim of reproduced results.

| Work | Primary technical novelty | Affective capability | Evidence / learning signal | Location |
|---|---|---|---|---|
| [Emotion-LLaMA](https://proceedings.neurips.cc/paper_files/paper/2024/hash/c7f43ada17acc234f568dc66da527418-Abstract-Conference.html) | Multimodal emotion-specific instruction tuning | Perception + Reasoning | Instruction data; audiovisual cues | Evidence / Learning |
| [UniMER](https://aclanthology.org/2026.emnlp-main.1611/) | Language-interface multimodal inputs, prototype-attention pooling, parameter-efficient transfer | Perception | Image/acoustic/facial cues converted to text; LoRA | Evidence / Learning |
| [SoVTR](https://aclanthology.org/2026.findings-emnlp.1807/) | Face/body/context attribute rewards for GRPO | Perception + Explanation | Attribute-level reward | Learning |
| [TMPO / HitEmotion](https://proceedings.iclr.cc/paper_files/paper/2026/hash/89ab43b626b480347dbaccda7be8aedb-Abstract-Conference.html) | ToM-guided process supervision | Reasoning | Mental-state supervision and reinforcement learning | Learning |
| [CogEmo](https://arxiv.org/abs/2610.11918) | Six cognitive appraisal dimensions, MoE adaptation, appraisal benchmark | Reasoning | Appraisal instruction data | Learning / Evaluation |
| [OPPO](https://openreview.net/forum?id=4dwe2wlxx5) | Omni-perception policy optimization | Reasoning | Cross-modal evidence and reasoning rewards | Learning |
| [OmniOPSD](https://arxiv.org/abs/2606.15920) | Rationale-privileged on-policy self-distillation | Reasoning | Rationale-guided distillation | Learning |
| [HMER / EHR](https://arxiv.org/abs/2609.11154) | Facet-specific hallucination evaluation and memory-guided logit rectification | Reasoning + Reliability | Hallucination and anchor memory | Inference / Evaluation |
| [LongEmo](https://arxiv.org/abs/2609.40079) | Query-specific retrieval from an Event Memory Graph | Long-horizon Reasoning | Episodic audiovisual memory | Inference |
| [CASE](https://arxiv.org/abs/2610.32481) | Emotion-pair-specific reusable skills for frozen MLLMs | Perception + Reasoning | Experience-driven skill library | Inference |
| [EmoMM / CHASE](https://aclanthology.org/2026.findings-acl.1018/) | Head-level attention steering under conflicting/missing modalities | Robust Perception | Inference-time conflict detection | Inference / Evidence |
| [TRACE-Streaming](https://aclanthology.org/2026.emnlp-main.554/) | Reliability-aware streaming emotion decisions and selective context reasoning | Temporal Understanding | Uncertainty and belief trajectory | Inference |
| [EmoOmni](https://arxiv.org/abs/2602.21900) | Omni-modal emotional understanding-to-expression | Generation + Interaction | Audio/video/text conditioning | Generation architecture |
| [EchoChat / EmpathyChat](https://arxiv.org/abs/2610.04826) | Staged cognitive reasoning for empathetic speech dialogues | Interaction + Speech Generation | Structured response supervision | Inference / Learning |
| [Emotion-Control Circuit](https://aclanthology.org/2026.emnlp-main.378/) | Activation-patching analysis of emotion transmission in LLM-based TTS | Speech Generation | Neuron/component causal interventions | Evidence / Interpretability |
| [FAB-G](https://arxiv.org/abs/2605.15755) | Salience selection from emotion-relevant visual attributes | Evoked emotion explanation | Attribute evidence and human salience annotations | Evidence / Inference |
| [MER-Bench](https://aclanthology.org/2026.emnlp-main.940/) | Benchmark for emotional reappraisal of image-text memes | Generation / Reappraisal | Multimodal editing criteria | Evaluation |
| [EmoS](https://aclanthology.org/2026.acl-long.1813/) | Fine-grained, continuous streaming emotion labels | Streaming Perception | Human-annotated emotional evolution | Evaluation |
| [AHaBench](https://aclanthology.org/2026.findings-eacl.4/) | Diagnoses affective hallucination and tests DPO safety | Text-only Interaction | Emotional enmeshment, presence illusion, overdependence | Adjacent Safety |
| [EIBench](https://aclanthology.org/2026.findings-emnlp.789/) | Simulator-based multi-turn emotion management and turn-credit RL | Text-only Interaction | Per-turn simulated state feedback | Adjacent Evaluation |

### Additional publisher-verified classification checks (2026-10-29)

| Work | Primary mechanism | Secondary link | Verification boundary |
|---|---|---|---|
| [ERV (AAAI 2026)](https://ojs.aaai.org/index.php/AAAI/article/view/37184) | **Learning:** explanation reward trains emotion--rationale coherence | Evaluation of explanatory coherence | Predicted-label agreement is not by itself modality-grounded faithfulness |
| [CAIR (ACL Findings 2026)](https://aclanthology.org/2026.findings-acl.1263/) | **Learning:** causal-mediation reward and adaptive RL | Cognitive appraisal and interventional evaluation | Rationale predictive contribution does not prove psychological causality |
| [EMO-CoT (IEEE T-AFFC 2026)](https://doi.org/10.1109/TAFFC.2026.3713090) | **Learning:** SCoT-DPO preference optimization | Multi-granular evidence architecture; EMER-CoT dataset; GEM evaluator | Multi-part paper, counted once; graph-based evidence alignment is not actual model-causal attribution |
| [EMARF (Pattern Recognition 2026)](https://www.sciencedirect.com/science/article/pii/S0031320326003316) | **Learning:** lightweight LoRA-based reasoning adaptation | Runtime consistency-gated fast/stepwise inference | Its adaptive inference behavior is not a training-free method |

These cases support a method-level distinction among **(i) label correctness, (ii) rationale--emotion coherence, (iii) observational cue grounding, and (iv) intervention-based rationale contribution**. They should be compared using matched inputs, annotation targets and judge protocols. No single metric proves all four.

## 3. Research questions the survey should actually answer

**RQ1 — Affective evidence grounding.** Under modality conflict, does the answer rely on face, voice, linguistic semantics or scene context? Does the method validate the evidence it mentions?

**RQ2 — From classification to appraisal.** How is an emotion connected to an event appraisal, belief, goal, cause or consequence? Which evaluations distinguish grounded inference from plausible explanation?

**RQ3 — Learning-signal granularity.** Does optimization target final label accuracy, process-level affective evidence, human preferences, speech expression quality or interpersonal outcomes? What trade-offs appear?

**RQ4 — Inference-time adaptation and memory.** Can frozen MLLMs handle uncertain emotions by modifying evidence selection, inference trajectories, episodic retrieval or reusable skills?

**RQ5 — Affective expression and interaction.** What is the difference between producing a well-conditioned emotional signal, giving an appropriate empathetic response, and improving an interaction over multiple turns?

**RQ6 — Robust and safe evaluation.** What is measured: expressed emotion, perceived emotion, evoked emotion, subject-experienced emotion or external evaluator preference? How are cross-person/cross-cultural shifts, calibration and unwanted emotional dependency assessed?

## 4. Proposed paper structure (8 sections)

1. Introduction
2. Background and Taxonomy
3. Affective Evidence Modeling
4. Affective Learning and Optimization
5. Affective Reasoning, Inference and Interaction
6. Benchmarks and Evaluation
7. Challenges and Future Directions
8. Conclusion

**Open structural issue:** Section 5 includes both inference control and generative interaction; expand the response-generation literature before deciding whether to split or rename it. This decision should follow a paper-by-paper mapping, not author preference alone.

## 5. Figures and tables justified by this evidence

| Asset | Purpose | Checks |
|---|---|---|
| Fig. 1 | Motivation: signals → evidence → appraisal/reasoning → response | Clearly distinguish recognition from interaction |
| Fig. 2 | Main method taxonomy with the capability axis as tags | One principal branch per method; avoid training/inference overlap |
| Fig. 3 | Multimodal grounding and conflict handling mechanisms | Show evidence flow and hallucination failure modes |
| Fig. 4 | RL / SFT / preference / distillation mechanisms | Identify the exact feedback optimized |
| Fig. 5 | Runtime reasoning, memory, verification and response generation | Include a genuine generative example |
| Table 1 | Existing survey scope and classification comparison | Use exact sections from prior surveys |
| Table 2 | Models: modalities, backbones, optimization, tasks | Only verified source data |
| Table 3 | Benchmark capabilities and evaluation metrics | Never merge incomparable tasks |
| Table 4 | Method × capability × learning signal × evidence setting | Report absence as unverified, not a negative result |

## 6. Current coverage and limitations

The companion README is a **bibliographic index**, not a systematic review. The CSV retains one canonical record per publication, while README may cross-list model and dataset names. No experimental performance table should be constructed from the abstract-only screening pass.

Priorities for the next reading pass: **SoVTR, TMPO, CogEmo, HMER, CASE, LongEmo, TRACE-Streaming, Emotion-Control Circuit, EmoOmni, and EchoChat**.

