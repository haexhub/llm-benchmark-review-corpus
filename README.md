# LLM Benchmark Review Corpus

Public development and calibration fixtures for reproducible AI code-review
benchmarks. Each item is a Git bundle containing a Base/Head PR pair plus a
public manifest. This repository deliberately contains no Gold labels,
reproducers, reference fixes or private source material.

Decision-grade Oracle material lives in the private companion repository
`haexhub/llm-benchmark-review-oracle` and is mounted only for post-run
evaluation.

`review-corpus/review-v1` has 102 curator-approved items (82 seeded across
correctness/security/performance/error_handling/testing/configuration, 20 clean
controls; Python and TypeScript). 16 items are real historical bugs from public
repositories (see each item's `approval_ref` for the originating commit); 86 are
synthetic. All Gold labels are decision-ready. It does not yet split out
calibration or holdout partitions — everything is currently `partition: development`.
Public development and calibration corpus for reproducible AI code-review benchmarks
