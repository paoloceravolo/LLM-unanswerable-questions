**(1) Yin et al., 2023 – “Do Large Language Models Know What They Don’t Know?”** ([arXiv](https://arxiv.org/abs/2305.18153))

- Introduces **self-knowledge** as “understanding their own limitations on the unknowns”.
- Focuses on **unanswerable or unknowable questions**, and on whether models can *recognize* them.
- Builds **SelfAware**, a dataset of unanswerable questions “from five diverse categories” plus answerable counterparts. ([arXiv](https://arxiv.org/abs/2305.18153))

**(2) Wen et al., 2025 – “Know Your Limits: A Survey of Abstention in Large Language Models”** ([arXiv](https://arxiv.org/html/2407.18418))

- Defines **abstention** as *refusal to answer*, including a spectrum from explicit “I don’t know” to hedged/partial replies. ([arXiv](https://arxiv.org/html/2407.18418))
- Proposes a **three-perspective framework** for when questions should not be answered:
  - **Query perspective**: ambiguous, incomplete, beyond human knowledge, insufficient or conflicting evidence. ([arXiv](https://arxiv.org/html/2407.18418))
  - **Model-knowledge perspective**: model is not confident or likely to be wrong. ([arXiv](https://arxiv.org/html/2407.18418))
  - **Human-values perspective**: answering would violate safety, privacy, fairness, etc., or anthropomorphize the model. ([arXiv](https://arxiv.org/html/2407.18418))

**(3) Chen et al., 2024 – “See What LLMs Cannot Answer: A Self-Challenge Framework for Uncovering LLM Weaknesses”** ([arXiv](https://arxiv.org/html/2408.08978))

- Starts from **failure instances** and has GPT-4 summarize **error patterns** that characterize queries it fails on.
- After human-in-the-loop refinement, they obtain **8 error patterns** (e.g., text manipulation, temporal ambiguity, questions with hidden assumptions). ([arXiv](https://arxiv.org/html/2408.08978))
- Builds **SC-G4**, a benchmark of 1,835 “self-challenging” queries where GPT-4 only reaches ~45% accuracy. ([arXiv](https://arxiv.org/html/2408.08978))

**(4) Suresh et al., 2024 – “Do LLMs Know When to NOT Answer? Investigating Abstention Abilities…”** ([arXiv](https://arxiv.org/html/2407.16221v1))

- Explicitly distinguishes **answerable vs unanswerable** MCQ items.
- Introduces **Abstain-QA**, a dataset with an equal split of answerable/unanswerable questions and an explicit IDK/NOTA option. ([arXiv](https://arxiv.org/html/2407.16221v1))
- Defines
  - **Abstention rate** (how often the model abstains)
  - **Answerable Accuracy** (accuracy when the question *is* answerable)
  - **Unanswerable Accuracy** (how often it correctly abstains on unanswerable items). ([arXiv](https://arxiv.org/html/2407.16221v1))
- Uses an **Answerable-Unanswerable Confusion Matrix (AUCM)** to analyze true/false positives/negatives across answerable/unanswerable × abstain/answer. ([arXiv](https://arxiv.org/html/2407.16221v1))

**(5) “Answering the Unanswerable Is to Err Knowingly” (2025)** ([arXiv](https://arxiv.org/pdf/2508.18760?utm_source=chatgpt.com))

- Shows that some LLMs internally recognize that a question is **unanswerable**, yet still produce an answer instead of abstaining.
- Frames this as a misalignment between **internal cognition** and **external output**, i.e., *knowing* something is unanswerable but failing to act accordingly. ([arXiv](https://arxiv.org/pdf/2508.18760?utm_source=chatgpt.com))
