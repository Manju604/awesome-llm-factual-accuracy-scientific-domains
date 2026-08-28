# Curated Research Papers
Verified against publisher pages, ACL Anthology, arXiv, Semantic Scholar, or PubMed. See `citation-audit/Citation_Integrity_Audit.md` for the verification log covering the papers cited directly in the survey.

## Survey and Review Papers
- **Survey of Hallucination in Natural Language Generation**
  Ji, Z., Lee, N., Frieske, R., et al., 2023, *ACM Computing Surveys*, 55(12), 1–38
  [DOI](https://doi.org/10.1145/3571730)
  Foundational taxonomy distinguishing intrinsic/extrinsic hallucination, cited throughout the survey's background section.

- **A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions**
  Huang, L., Yu, W., Ma, W., et al., 2025, *ACM Transactions on Information Systems*, 43(2), 1–55
  [DOI](https://doi.org/10.1145/3703155) · [arXiv:2311.05232](https://arxiv.org/abs/2311.05232)
  Distinguishes factuality hallucination from faithfulness hallucination and catalogues mitigation techniques.

- **Survey on Factuality in Large Language Models: Knowledge, Retrieval and Domain-Specificity**
  Yang, L., Wang, J., Xie, X., Zhang, Z., & Zhang, Y., 2025, *ACM Computing Surveys*
  [DOI](https://doi.org/10.1145/3742420) · [arXiv:2310.07521](https://arxiv.org/abs/2310.07521)
  Surveys factuality along knowledge storage, retrieval, and domain-specificity axes.

- **Factuality of Large Language Models: A Survey**
  Wang, Y., Wang, M., Manzoor, M. A., et al., 2024, arXiv:2402.02420
  [arXiv](https://doi.org/10.48550/arXiv.2402.02420)
  Catalogues post-2023 factuality benchmarks by discrimination vs. generation task type.

## Foundational (General-Purpose) Benchmarks
- **Measuring Massive Multitask Language Understanding (MMLU)**
  Hendrycks, D., Burns, C., Basart, S., et al., 2021, ICLR 2021, arXiv:2009.03300
  [arXiv](https://doi.org/10.48550/arXiv.2009.03300)
  57-subject multitask benchmark; the near-universal STEM/general-knowledge reporting standard that scientific benchmarks are compared against.

- **TruthfulQA: Measuring How Models Mimic Human Falsehoods**
  Lin, S., Hilton, J., & Evans, O., 2022, ACL 2022, pp. 3214–3252
  [DOI](https://doi.org/10.18653/v1/2022.acl-long.229) · [arXiv:2109.07958](https://arxiv.org/abs/2109.07958)
  817 questions across 38 categories; showed larger models can be less truthful by reproducing imitative falsehoods.

- **MMLU-Pro: A More Robust and Challenging Multi-Task Language Understanding Benchmark**
  Wang, Y., Ma, X., Zhang, G., et al., 2024, NeurIPS 2024, arXiv:2406.01574
  [arXiv](https://arxiv.org/abs/2406.01574)
  Harder successor to MMLU built to counter ceiling/saturation effects.

- **Measuring Short-Form Factuality in Large Language Models (SimpleQA)**
  Wei, J., Karina, N., Chung, H. W., et al., 2024, arXiv:2411.04368
  [arXiv](https://doi.org/10.48550/arXiv.2411.04368)
  Adversarially collected short-answer factuality probe with explicit reward for calibrated abstention.

## Domain-Specific Benchmarks — Medicine
- **Large Language Models Encode Clinical Knowledge (MultiMedQA / Med-PaLM)**
  Singhal, K., Azizi, S., Tu, T., et al., 2023, *Nature*, 620, 172–180
  [DOI](https://doi.org/10.1038/s41586-023-06291-2) · [arXiv:2212.13138](https://arxiv.org/abs/2212.13138)
  Combines six medical QA datasets plus a new consumer-query set; proposes a multi-axis human evaluation rubric.

- **Toward Expert-Level Medical Question Answering with Large Language Models (Med-PaLM 2)**
  Nature Medicine, 2024
  [Nature Medicine](https://www.nature.com/articles/s41591-024-03423-7)
  Follow-up work showing gains over Med-PaLM on the same MultiMedQA suite, assessed by physicians and laypeople.

- **PubMedQA: A Dataset for Biomedical Research Question Answering**
  Jin, Q., et al., 2019
  [GitHub](https://github.com/pubmedqa/pubmedqa) · [Hugging Face](https://huggingface.co/datasets/qiaojin/PubMedQA)
  Yes/no/maybe QA over PubMed abstracts; one of the six datasets aggregated into MultiMedQA.

## Domain-Specific Benchmarks — Chemistry
- **A Framework for Evaluating the Chemical Knowledge and Reasoning Abilities of Large Language Models Against the Expertise of Chemists (ChemBench)**
  Mirza, A., Alampara, N., Kunchapu, S., et al., 2025, *Nature Chemistry*, 17(7), 1027–1034
  [DOI](https://doi.org/10.1038/s41557-025-01815-x)
  2,700+ curated Q&A pairs across nine chemistry sub-domains, benchmarked against practicing chemists.

## Domain-Specific Benchmarks — Physics, Biology, Cross-Disciplinary
- **GPQA: A Graduate-Level Google-Proof Q&A Benchmark**
  Rein, D., Hou, B. L., Stickland, A. C., et al., 2023, arXiv:2311.12022
  [arXiv](https://doi.org/10.48550/arXiv.2311.12022)
  448 expert-validated multiple-choice questions in biology, physics, and chemistry, explicitly designed to resist web search.

## Scientific Claim Verification
- **Fact or Fiction: Verifying Scientific Claims (SciFact)**
  Wadden, D., Lin, S., Lo, K., et al., 2020, EMNLP 2020, pp. 7534–7550
  [DOI](https://doi.org/10.18653/v1/2020.emnlp-main.609)
  1,409 expert-written biomedical claims paired with a 5,183-abstract evidence corpus, labeled SUPPORTS/REFUTES/NOT-ENOUGH-INFO.

- **SciFact-Open: Towards Open-Domain Scientific Claim Verification**
  Wadden, D., Lo, K., Kuehl, B., et al., 2022, Findings of ACL: EMNLP 2022, pp. 4719–4734
  [ACL Anthology](https://aclanthology.org/2022.findings-emnlp.347/)
  Expands the SciFact evidence corpus to ~500,000 abstracts to reflect open-domain retrieval difficulty.

- **Explaining Health Claims: A Dataset for Evidence-Based Fact-Checking of Health-Related Claims (PubHealth)**
  Kotonya, N., & Toni, F., 2020
  [ACL Anthology](https://aclanthology.org/2020.emnlp-main.623/)
  ~11,800 journalist/fact-checker-authored public-health claims, extending claim verification beyond peer-reviewed literature alone.

- **Evidence-Based Fact-Checking of Health-Related Claims (HealthVer)**
  Sarrouti, M., Abacha, A. B., M'rabet, Y., & Demner-Fushman, D., 2021, Findings of EMNLP 2021
  [ACL Anthology](https://aclanthology.org/2021.findings-emnlp.297/)
  ~1,800 claims extracted from real health-related search queries, evaluated against evidence abstracts.

- **SciTab: A Challenging Benchmark for Compositional Reasoning and Claim Verification Using Scientific Tables**
  Lu, X., Pan, L., Liu, Q., Nakov, P., & Kan, M.-Y., 2023, EMNLP 2023
  [ACL Anthology](https://aclanthology.org/2023.emnlp-main.483/)
  Extends the claim-verification paradigm to compositional reasoning over tables in computer-science papers.

- **COVID-Fact: Fact Extraction and Verification of Real-World Claims on COVID-19 Pandemic**
  Saakyan, A., Chakrabarty, T., & Muresan, S., 2021, ACL-IJCNLP 2021
  [ACL Anthology](https://aclanthology.org/2021.acl-long.165/)
  ~4,000 claims from Reddit paired with generated counterclaims, extending SciFact-style verification to a fast-moving public-health topic.

## Evaluation Methodology / Fine-Grained Scoring
- **FActScore: Fine-Grained Atomic Evaluation of Factual Precision in Long Form Text Generation**
  Min, S., Krishna, K., Lyu, X., et al., 2023, EMNLP 2023, pp. 12076–12100
  [DOI](https://doi.org/10.18653/v1/2023.emnlp-main.741) · [arXiv:2305.14251](https://arxiv.org/abs/2305.14251)
  Decomposes long-form generations into atomic facts and scores the percentage supported by a trusted knowledge source.

- **SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models**
  Manakul, P., Liusie, A., & Gales, M., 2023, EMNLP 2023, arXiv:2303.08896
  [arXiv](https://arxiv.org/abs/2303.08896)
  Sampling-based, zero-resource method that flags hallucinated sentences via consistency across multiple generations — a knowledge-source-free complement to FActScore.
