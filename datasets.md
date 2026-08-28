# Datasets

- **GPQA (Graduate-Level Google-Proof Q&A)**
  Source: [Hugging Face — idavidrein/gpqa](https://huggingface.co/datasets/idavidrein/gpqa) · [GitHub](https://github.com/idavidrein/gpqa)
  Description: 448 multiple-choice questions in biology, physics, and chemistry, written and validated by domain experts and checked for resistance to web search.
  Use: Stress-testing parametric scientific knowledge and reasoning in a contamination-resistant, expert-level setting.

- **SciFact**
  Source: [Hugging Face — allenai/scifact](https://huggingface.co/datasets/allenai/scifact) · [GitHub](https://github.com/allenai/scifact)
  Description: 1,409 expert-written biomedical claims paired with a 5,183-abstract evidence corpus, labeled SUPPORTS / REFUTES / NOT-ENOUGH-INFO.
  Use: Training and evaluating literature-grounded scientific claim-verification systems rather than pure recall QA.

- **PubMedQA**
  Source: [GitHub — pubmedqa/pubmedqa](https://github.com/pubmedqa/pubmedqa) · [Hugging Face — qiaojin/PubMedQA](https://huggingface.co/datasets/qiaojin/PubMedQA)
  Description: Yes/no/maybe biomedical question answering derived from PubMed abstract titles and conclusions, with labeled (1k), unlabeled (61.2k), and artificially generated (211.3k) subsets.
  Use: One of the six datasets aggregated into MultiMedQA; used to evaluate quantitative, literature-grounded biomedical reasoning.

> Note: If your own project only needs a subset of these, keep the three above (they satisfy the assignment's minimum of 3) and add domain-specific datasets you use directly (e.g. MedQA/USMLE-style sets, MedMCQA) as your work progresses.
