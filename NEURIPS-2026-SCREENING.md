# NeurIPS 2026 — Affective Intelligence Screening Queue

**Screening date:** 2026-10-29  
**Official indexed source:** [NeurIPS 2026 Downloads / paper-name list](https://neurips.cc/Downloads/2026). The title listing is **not** an individual proceedings/abstract page. Some results from `dev.neurips.cc` may reflect an earlier snapshot and must be cross-checked against the finalized program.

This queue is separate from the [canonical bibliography](papers.csv). **Do not count candidate rows as verified independent papers** until title, venue and research scope can be confirmed from a full paper or authoritative abstract.

## A. Already indexed in the core/adjacent bibliography

| Work | Verified scope | Where it belongs |
|---|---|---|
| [AffectGPT-RL](https://arxiv.org/abs/2605.06126) | RL for open-vocabulary emotion recognition; conference title listed | Core: Learning and Optimization |
| [EchoChat (conference-list title EmpathyChat)](https://arxiv.org/abs/2610.04826) | Structured reasoning for spoken empathetic dialogue; *one paper despite name difference* | Core: Inference / Interaction |
| [CAREBench](https://arxiv.org/abs/2605.17176) | Cognitive appraisal benchmark for **text LLMs** | Adjacent benchmark; not MLLM |
| [Affective AI Safety](https://arxiv.org/abs/2606.23380) | Affective AI safety perspective / position | Adjacent safety, not a core MLLM method |

## B. Additional NeurIPS title candidates — full-paper verification needed

| Title from NeurIPS list | Why it warrants review | Evidence needed before inclusion |
|---|---|---|
| **Accessing Emotion Within: Tracing Latent Affective Cues in Multimodal Large Language Models** | Directly relevant to MLLM affective representations and mechanistic interpretability | Obtain exact paper/abstract, modalities, intervention type, full author list |
| **Omni-ECD: Omni Emotion Cause Derivation in Conversation** | Potentially extends multimodal emotional-cause reasoning | Determine whether an LLM/MLLM is actually used; check benchmark and reasoning mechanism |
| **AffectAtlas: Structured and Neuro-Symbolic Affect Modeling for Emotionally Consistent Talking Face Generation** | Emotion-conditioned audiovisual generation | Determine whether core architecture uses an LLM or is non-LLM generative vision/audio |
| **Affective Adaptive Interaction Strategy for ASD Companion Social Robots via LLM-Driven Simulation** | Affective multi-turn agents and embodied interaction | Confirm publication type, multimodal inputs, task evaluation and LLM role |
| **CausalAffect: Causally Guided Learning of Psychology-Aligned Facial Affect Relations** | Causal affect representation and psychology-grounded explanation | Author descriptions indicate a primarily CV facial-action-unit model; **likely adjacent rather than core MLLM** |
| **Emotion-Trained Vision Models Do Not Necessarily Learn EEG-Aligned Facial Dynamics** | Cross-modal affect representation validity | Determine whether LLM appears; otherwise adjacent empirical background |
| **Enhancing LLMs with Cognitive-Affective Personality Inference for Simulating Human Social-Psychological Behavior** | Personality and emotional reasoning in agents | Appears text-oriented; mark adjacent unless multimodal basis verified |

## C. Inclusion decisions and confidence

**Already verified core:** AffectGPT-RL; EchoChat / EmpathyChat (title discrepancy noted).  
**Strong priority for full-paper lookup:** Accessing Emotion Within; Omni-ECD.  
**Conditional / likely adjacent:** AffectAtlas; Affective Adaptive Interaction Strategy; CausalAffect; Emotion-Trained Vision Models; Personality Inference.

**Conservative rule:** Official paper-name listing verifies the *title's presence*, not its technical claim or applicability to our MLLM taxonomy. Do not invent an arXiv ID or code link when none is established.

## D. Reading questions for the two highest-priority candidates

1. Does **Accessing Emotion Within** causally intervene on affect features in an MLLM or just probe correlated activations?
2. Does **Omni-ECD** jointly use video, speech and text, and what role does generative language reasoning play?
3. Do they provide *evidence-grounded* emotion evaluations or just label accuracy?
4. Are there publicly available benchmark splits, released code, or source labels?
5. How do their contributions compare with TMPO, HMER, CogEmo, EmotionHallucer and SoVTR?

The queue is deliberately narrower than the complete NeurIPS program; it prioritizes papers that could change the survey's technical taxonomy.
