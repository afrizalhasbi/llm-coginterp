# TODO

## Data cleanup
- [ ] Deduplicate models with multiple model_id/model_name entries (same model, different aliases)
- [ ] Remove experimental/inproper model entries (e.g., names describing training steps rather than model identity)
- [ ] Run verify_data.py after any data changes to ensure FK integrity

## Data expansion — large extraction tasks

### Stanford HELM
- [ ] Extract Stanford HELM data per individual benchmark across all HELM sub-projects (Safety, Audio, Image2Struct, Reasoning, Long-Context, MMLU-Winogrande-Afr, MedHELM, ThaiExam, TORR, EWoK, Finance, Arabic Enterprise, SEA-HELM, etc.)
- [ ] Extract per-benchmark scores, NOT mean/aggregate scores averaged across benchmark groups
- [ ] Follow existing methodology (strict source verification, model inclusion criteria, normalization rules)

### Kaggle Benchmarks
- [ ] Extract all benchmarks from Kaggle Research category (104 benchmarks as of 2026-06-16)
- Source: https://www.kaggle.com/benchmarks/?browse=true&type=research
- [ ] Extract per-benchmark model scores individually
- [ ] Follow existing methodology

### Papers With Code
- [ ] Extract benchmarks from Papers With Code tasks page
- Source: https://paperswithcode.co/tasks — iterate through every topic/subtask that has associated benchmarks
- [ ] Extract per-benchmark model scores individually
- [ ] Follow existing methodology

### Previous HELM sweep (lost)
- [x] ~~HELM sweep data (312 benchmarks, 1155 models, 11208 results) extracted locally but not yet committed~~ — Data was lost (never committed to git). Re-extract via tasks above.

## Methodology updates
- [ ] Add to METHODOLOGY.md: If there is more than 1 score for the same model in a benchmark (due to different setup, different provider/evaluator running the benchmark, etc.), keep each as a **separate row** in results.csv rather than averaging. Distinguish rows via the `setup` and `source_url` fields.

## Scripts (needs refactor before committing to repo)
- [ ] Refactor scripts/ directory — consolidate duplicate checkers (check_dupes.py, check_dupes2.py), clean up one-off scripts
- [ ] Add docstrings and CLI help to all utility scripts
- [ ] benchmark_analysis.md — refactor analysis output into proper report format

## Documentation
- [ ] Expand README with usage examples and data schema reference
- [ ] Add CONTRIBUTING.md if opening to collaborators
