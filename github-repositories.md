# GitHub Implementations

- **idavidrein/gpqa**
  [github.com/idavidrein/gpqa](https://github.com/idavidrein/gpqa)
  What it implements: The official GPQA dataset release plus baseline evaluation scripts (zero-shot, few-shot, chain-of-thought, retrieval-augmented) for GPT-3.5/GPT-4.
  Why relevant: Canonical reference implementation for the cross-disciplinary graduate-level benchmark discussed in Section 4.3 of the survey.

- **allenai/scifact**
  [github.com/allenai/scifact](https://github.com/allenai/scifact)
  What it implements: Data loaders, baseline claim-verification models, and evaluation scripts for the SciFact task, plus a public AI2 leaderboard.
  Why relevant: Reference implementation for the literature-grounded claim-verification paradigm discussed in Section 4.4.

- **dwadden/multivers**
  [github.com/dwadden/multivers](https://github.com/dwadden/multivers)
  What it implements: MultiVerS, a Longformer-based model achieving state-of-the-art results on SciFact, CovidFact, and HealthVer simultaneously, with training and inference code and checkpoints.
  Why relevant: Shows how one architecture generalizes across multiple scientific claim-verification datasets referenced in the survey's Section 4.4.

- **lamalab-org/chembench**
  [github.com/lamalab-org/chembench](https://github.com/lamalab-org/chembench) · [project site](https://lamalab-org.github.io/chembench/)
  What it implements: The full ChemBench evaluation framework — question sets, automated grading, refusal counting, and a public leaderboard — actively maintained (MIT license) by LamaLab, University of Jena.
  Why relevant: Official implementation of the chemistry benchmark discussed in Sections 4.2 and 5.3–5.4 of the survey.

- **shmsw25/FActScore**
  [github.com/shmsw25/FActScore](https://github.com/shmsw25/FActScore)
  What it implements: The retrieval-plus-LLM pipeline that automates atomic-fact factual-precision scoring, reproducing the paper's <2% error rate relative to human annotation.
  Why relevant: Reference implementation for the atomic fact decomposition methodology discussed in Section 3.2 of the survey.

- **confident-ai/deepeval**
  [github.com/confident-ai/deepeval](https://github.com/confident-ai/deepeval)
  What it implements: A general-purpose, actively maintained LLM evaluation framework with a dedicated hallucination metric and 50+ other metrics for RAG, agents, and long-form generation.
  Why relevant: Illustrates how atomic/claim-based factuality scoring (Section 3.2–3.3) has been productionized into reusable tooling beyond the original research code.
