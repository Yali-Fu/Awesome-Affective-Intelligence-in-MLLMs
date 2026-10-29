# Literature curation protocol

**Maintainer:** Yali Fu  
**Scope:** Affective Intelligence in Multimodal Large Language Models  
**Last checked:** 2026-10-29

This repository is a bibliography and research-organizing aid. Inclusion does not indicate endorsement or that all authors/repository maintainers have read the full paper.

## Eligibility

1. **Core method:** A language-based foundation model (MLLM, audio-language model, omni-modal LLM, or LLM-centered multimodal system) is part of the affective learning, understanding, generation, or response pipeline.
2. **Benchmark:** A benchmark measures emotion or empathy capabilities of LLMs/MLLMs, with explicit model/task applicability.
3. **Adjacent:** Important text-only empathy/affect research, cognition or emotion theory, safety, or earlier non-MLLM multimodal research. This must be labeled as adjacent rather than silently counted as an MLLM method.
4. **Survey:** Surveys of multimodal emotion recognition, reasoning, generation, or LLM affective computation.

## Required metadata before adding

- Exact **paper title** from arXiv or the official publisher.
- **Year, current publication venue/status**, and a primary paper link.
- Distinct **Official / arXiv / GitHub / Hugging Face** links, when confirmed.
- Main input modalities (Text, Image, Video, Audio, physiological data) and generated outputs.
- Primary **method mechanism** (Representation/Alignment, Learning/Optimization, Inference/Interaction).
- Main **affective capability** (Perception, Understanding, Reasoning, Generation, Interaction).
- Type: **Core Method / Benchmark / Survey / Adjacent**.
- Provenance: `Seed` (in original notes) or `New` (identified independently).
- Check whether another record already corresponds to the same arXiv ID or officially retitled work.

## Venue and link rules

- Do not infer acceptance from the paper's arXiv year, unverified blog posts, or an outdated abstract.
- If an individual proceedings page is unavailable, link to the official indexed paper list and mark it explicitly **conference paper list**.
- Track paper renamings (e.g., the NeurIPS 2026 listing **EmpathyChat** vs. arXiv/author-site **EchoChat**) without double counting.
- Do not fabricate code, weights, datasets, results or exact GPU budgets.
- Keep exact paper titles. Method names are discovery aids, not part of the paper's official title unless they appear there.
- For GitHub entry titles, prefer `Year_Venue_MethodName_Full-Title` when preparing individual future markdown notes. Do not encode a false venue to satisfy this convention.

## Quality assurance before writing the survey

- **Paper-level:** Read method, dataset construction, evaluation protocol, training resources, baselines, limitations and supplementary material.
- **Experiment-level:** Do not aggregate metrics across distinct tasks, modality settings, validation/test protocols, splits or LLM-as-a-judge conditions.
- **Taxonomy-level:** Choose one *primary* method section; retain secondary capability and learning-signal tags. Reclassify when a careful reading shows the primary contribution is different.
- **Research gap analysis:** Distinguish *expressed*, *perceived*, *evoked* and *experienced* emotion; avoid conflating subjective emotional ratings with objective labels.
- **Reference accuracy:** Generate BibTeX from the publisher/arXiv rather than guessing conference bib metadata.

## Suggested pull-request template

- Paper:
- Official / arXiv:
- Venue/status and verification link:
- Method category:
- Capability and modality tags:
- Main contribution (one or two evidence-grounded sentences):
- Code / dataset links:
- Duplicate check:
- Notes on uncertainty:
