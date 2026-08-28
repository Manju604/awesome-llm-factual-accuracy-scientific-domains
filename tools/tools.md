# Tools and Libraries

- **FActScore (PyPI package)**
  [GitHub](https://github.com/shmsw25/FActScore) — Official implementation accompanying Min et al. (2023). Computes atomic-fact factual-precision scores for long-form LLM generations against a retrieval knowledge source. Install via `pip install factscore`.

- **SelfCheckGPT**
  [GitHub](https://github.com/potsawee/selfcheckgpt) — Official implementation accompanying Manakul et al. (2023). Zero-resource, sampling-based hallucination detection that flags sentences with high inconsistency across repeated generations from the same model.

- **DeepEval**
  [GitHub](https://github.com/confident-ai/deepeval) — Open-source, pytest-style LLM evaluation framework with built-in hallucination, faithfulness, and contextual-relevancy metrics for RAG and long-form generation.

- **RAGAS**
  [Documentation](https://docs.ragas.io/) — Reference-free evaluation framework for retrieval-augmented pipelines; its faithfulness metric performs automated claim verification of generated answers against retrieved context, directly relevant to grounding scientific answers in literature.

- **TruLens**
  [Documentation](https://www.trulens.org/) — Provides a "groundedness" feedback function for scoring whether generated text is supported by retrieved context, usable for auditing retrieval-augmented scientific QA pipelines.

> Verification note: RAGAS and TruLens homepages were checked via web search summaries rather than opened directly in this session — re-confirm their current documentation URLs before final submission, consistent with this repository's citation-integrity practice.
