# Changelog

All notable changes to the LLM Benchmarks dataset.

---

## [Unreleased]

### Added
- EmoBench results
- EQ-Bench results

### Fixed
- Blank `score` column: All previously blank rows now have scores filled in

---

## Process Group 4 — Morality/Ethics Batch

### Added
- MoralBench results
- Moral Machine for LLMs results
- AITA Normative Evaluation results

### Removed
- ETHICS (no valid LLM baseline scores)
- Value Kaleidoscope (no valid LLM baseline scores)
- Delphi (no valid LLM baseline scores)

---

## Process Group 3 — Humor/Creativity Batch

### Added
- HumorBench results
- Not All Jokes Land (workplacehumor) results
- LitBench results
- CreativityPrism results

### Purged (re-added later)
- Oogiri LLM Benchmark (re-added in Group 3.5)
- TTCW (re-added in Group 3.5)
- CS4
- A Confederacy of Models

---

## Process Group 2 — Games/Strategy + Others

### Added
- LLM Chess results
- GTBench results
- RPGBench results

### Removed
- Readable Minds (not a standard LLM benchmark)
- LudoBench (not a standard LLM benchmark)
- gg-bench (not a standard LLM benchmark)
- PokerBench (not a standard LLM benchmark)

---

## Earlier Work

### HF Open LLM Leaderboard Cleanup ✓
- v1 and v2 leaderboard rows retained as-is
- v2 collected with "Only Official Providers" filter
- v1 reviewed and confirmed acceptable

### Blank Score Filling ✓
- 21 of 57 blank-score rows filled
- 36 intentionally blank (documented reasons in TODO.md)

### Baseline Model Expansion
- Added exhaustive SOTOPIA results
- Added exhaustive SI-Bench and ELEPHANT results
- Updated EQ-Bench and EmoBench exports
