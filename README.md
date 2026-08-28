# Awesome LLM Factual Accuracy in Scientific Domains

A curated, verified collection of research, datasets, and tools for benchmarking the factual accuracy of large language models in scientific domains.

## Contents
- [Overview](#overview)
- [AI-Assisted Research Paper](#ai-assisted-research-paper)
- [Curated Research Papers](#curated-research-papers)
- [Datasets](#datasets)
- [Tools and Libraries](#tools-and-libraries)
- [GitHub Implementations](#github-implementations)
- [Citation Integrity Audit](#citation-integrity-audit)
- [License](#license)

## Overview
Large language models are increasingly consulted for scientific information spanning medicine, chemistry, physics, and biology, yet they remain prone to generating fluent but factually incorrect content. This repository curates the research, benchmarks, datasets, and tooling used to measure that factual reliability. It traces the field from general-purpose truthfulness probes (TruthfulQA, MMLU) to domain-specialized instruments (MultiMedQA/Med-PaLM for medicine, ChemBench for chemistry, GPQA across physics/biology/chemistry, SciFact for biomedical claim verification), and from coarse accuracy scoring to fine-grained methodologies such as atomic fact decomposition (FActScore) and adversarial short-form factuality probes (SimpleQA). All resources here have been independently checked against primary or indexing sources rather than accepted directly from AI-generated suggestions — see the citation audit for the verification log.

## AI-Assisted Research Paper
[View Paper](paper/Benchmarking_LLM_Factual_Accuracy_Scientific_Domains.docx)
*Benchmarking Factual Accuracy of Large Language Models Across Scientific Domains: A Review and Synthesis of Evaluation Methodologies, Benchmarks, and Open Problems.* A review synthesizing benchmark design (multiple-choice, short-form, claim-verification), scoring methodology, and open research gaps (contamination, single-answer assumptions, expert-annotation cost, multilingual/multimodal coverage) in scientific factuality evaluation.

## Curated Research Papers
20 verified papers organized by category — see [`references/references.md`](references/references.md) for full citations, links, and relevance notes:
- Survey and Review Papers (4)
- Foundational (General-Purpose) Benchmarks (4)
- Domain-Specific Benchmarks — Medicine (3), Chemistry (1), Physics/Biology/Cross-Disciplinary (1)
- Scientific Claim Verification (6)
- Evaluation Methodology / Fine-Grained Scoring (2)

## Datasets
3 verified datasets — see [`datasets/datasets.md`](datasets/datasets.md): GPQA, SciFact, PubMedQA.

## Tools and Libraries
5 tools for measuring factuality and hallucination — see [`tools/tools.md`](tools/tools.md): FActScore, SelfCheckGPT, DeepEval, RAGAS, TruLens.

## GitHub Implementations
6 reference implementations — see [`implementations/github-repositories.md`](implementations/github-repositories.md): idavidrein/gpqa, allenai/scifact, dwadden/multivers, lamalab-org/chembench, shmsw25/FActScore, confident-ai/deepeval.

## Citation Integrity Audit
[View Audit](citation-audit/Citation_Integrity_Audit.md)
Every reference cited in the paper was checked for existence, correct authorship/year/venue, and matching DOI/arXiv ID. 5 of 13 were verified directly against a primary source; the remaining 8 were cross-confirmed indirectly and flagged for a final direct check before submission — see the audit for the full log and reasoning.

## License
This repository's original content (README, audit, and curation notes) is released under the [MIT License](LICENSE). Linked papers, datasets, and tools remain under their own respective licenses.
