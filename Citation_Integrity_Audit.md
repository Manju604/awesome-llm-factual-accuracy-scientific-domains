# Citation Integrity Audit
**Paper audited:** *Benchmarking Factual Accuracy of Large Language Models Across Scientific Domains: A Review and Synthesis of Evaluation Methodologies, Benchmarks, and Open Problems*
**Audit method:** Every in-text citation was opened directly at its primary or indexing source (ACL Anthology, arXiv, ACM Digital Library, NeurIPS/ICLR proceedings, Nature, PubMed) to confirm the paper exists and that title, authorship, year, venue, and DOI/arXiv ID match the claim made in the paper.

Status key: ✅ Verified directly against the primary source · ❌ Discrepancy found — needs correction in the paper.

| # | In-text citation | Verified title / venue | DOI or ID | Status |
|---|---|---|---|---|
| 1 | Rein et al., 2023 | GPQA: A Graduate-Level Google-Proof Q&A Benchmark — arXiv | 10.48550/arXiv.2311.12022 | ✅ |
| 2 | Mirza et al., 2025 | A framework for evaluating the chemical knowledge and reasoning abilities of LLMs against the expertise of chemists — *Nature Chemistry* 17(7), 1027–1034 | 10.1038/s41557-025-01815-x | ✅ |
| 3 | Wadden et al., 2020 | Fact or Fiction: Verifying Scientific Claims — EMNLP 2020, pp. 7534–7550 | 10.18653/v1/2020.emnlp-main.609 | ✅ |
| 4 | Singhal et al., 2023 | Large language models encode clinical knowledge — *Nature* 620, 172–180 | 10.1038/s41586-023-06291-2 | ✅ |
| 5 | Min et al., 2023 | FActScore: Fine-grained Atomic Evaluation of Factual Precision in Long Form Text Generation — EMNLP 2023, pp. 12076–12100 | 10.18653/v1/2023.emnlp-main.741 | ✅ |
| 6 | Hendrycks et al., 2021 | Measuring Massive Multitask Language Understanding — published as a conference paper at ICLR 2021 | arXiv:2009.03300 | ✅ |
| 7 | Lin, Hilton & Evans, 2022 | TruthfulQA: Measuring How Models Mimic Human Falsehoods — ACL 2022, pp. 3214–3252 | 10.18653/v1/2022.acl-long.229 | ✅ |
| 8 | Wei et al., 2024 | Measuring Short-Form Factuality in Large Language Models (SimpleQA) — arXiv | arXiv:2411.04368 | ✅ |
| 9 | Wang et al., 2024 | MMLU-Pro: A More Robust and Challenging Multi-Task Language Understanding Benchmark — NeurIPS 2024 (Datasets and Benchmarks Track) | arXiv:2406.01574 | ✅ |
| 10 | Ji et al., 2023 | Survey of Hallucination in Natural Language Generation — *ACM Computing Surveys* 55(12), Article 248, 1–38 | 10.1145/3571730 | ✅ |
| 11 | Huang et al., 2025 | A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions — *ACM Transactions on Information Systems* 43(2), Article 42, 1–55 | 10.1145/3703155 (arXiv:2311.05232) | ✅ |
| 12 | Wang et al., 2024 (factuality survey) | Factuality of Large Language Models: A Survey — EMNLP 2024, pp. 19519–19529 (Wang, Y., Wang, M., Manzoor, M. A., Liu, F., Georgiev, G., Das, R. J., Nakov, P.) | 10.18653/v1/2024.emnlp-main.1088 (arXiv:2402.02420) | ✅ (note: also published at EMNLP 2024, not only posted to arXiv — cite the peer-reviewed proceedings, not just the preprint) |
| 13 | Yang et al., 2025 | Survey on Factuality in Large Language Models: Knowledge, Retrieval and Domain-Specificity — *ACM Computing Surveys* 58(1), Article 13 | 10.1145/3742420 (arXiv:2310.07521) | ❌ **Authorship discrepancy — see below** |

## Discrepancy found (item 13)
The paper cites this source as **"Yang, L., Wang, J., Xie, X., Zhang, Z., & Zhang, Y. (2025)."** — implying Yang is the first/lead author.

The actual paper (confirmed at the ACM Digital Library, arXiv, and the authors' own GitHub repository) is:
**Wang, C., Liu, X., Yue, Y., Tang, X., Zhang, T., Jiayang, C., Yao, Y., Gao, W., Hu, X., Qi, Z., Wang, Y., Yang, L., Wang, J., Xie, X., Zhang, Z., & Zhang, Y. (2025). Survey on Factuality in Large Language Models: Knowledge, Retrieval and Domain-Specificity. *ACM Computing Surveys*, 58(1), Article 13.**

**Cunxiang Wang is the first author**, not Yang. The names "Yang, Wang, Xie, Zhang, Zhang" in the paper's citation are real co-authors, but they are the 12th-16th authors on the actual 16-author paper -- not the lead authors. This looks like a citation-formatting error (possibly an AI-assisted citation tool truncating/reordering a long author list) rather than a fabricated source -- the DOI, title, and venue are all correct; only the author attribution is wrong.
**Action required:** Correct the in-text citation and bibliography entry to `Wang et al., 2025`, not `Yang et al., 2025`.

## Findings
- All 13 sources cited in the paper correspond to real, identifiable, correctly-titled publications -- no fabricated or non-existent references were found.
- 12 of 13 citations were confirmed fully correct (title, authorship, year, venue, DOI/ID all match).
- 1 of 13 (item 13) has a genuine **author misattribution**: the in-text citation names the wrong lead author for an otherwise correctly identified source. This is exactly the kind of error this audit is designed to catch, and should be fixed before the repository is submitted.
- Minor note (item 12): that source has since been published at EMNLP 2024 in addition to its arXiv posting; citing the peer-reviewed proceedings (10.18653/v1/2024.emnlp-main.1088) is preferable to citing only the arXiv preprint.
- Numerical claims spot-checked against source abstracts and confirmed accurate: GPQA's 39% GPT-4 baseline vs. 65-74% PhD-expert / 34% skilled-non-expert accuracy; ChemBench's 2,700+ curated question-answer pairs; FActScore's ~58% ChatGPT factual precision with <2% automated-metric error rate; MultiMedQA/Med-PaLM's 67.6% Flan-PaLM accuracy on MedQA (>17-point improvement over prior state of the art); TruthfulQA's 817 questions across 38 categories; MMLU's 57 tasks; MMLU-Pro's 16-33 percentage-point accuracy drop relative to MMLU.

## Recommendation
Fix the author attribution for item 13 (`Yang et al., 2025` to `Wang et al., 2025`) in both the in-text citation and the reference list before final submission. Optionally update item 12's citation to point to the EMNLP 2024 proceedings rather than the arXiv preprint.
