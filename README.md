# Toyc-benchmark

Toyc pip library **[toyc](https://github.com/spy1345a/toyc-repo)**,
a toy expression compiler with CPU and Vulkan GPU backends. This repo
holds the experiments; the library under study lives in toyc.

> **Paper:** *toyc: Data-Parallel Arithmetic Evaluation on Vulkan Compute for Expression Compilation*
> [![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.23853006-blue?style=flat-square)](https://doi.org/10.5281/zenodo.23853006) [![Library](https://img.shields.io/badge/Library-spy1345a%2Ftoyc--repo-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/spy1345a/toyc-repo)

## Run

```bash
pip install -r requirements.txt
```
```python
python example.py    # minimal usage demo, CSVs + summary
```

For software used look at `SYSTEM_INFO.txt`

For benchmark data go to `data/` — it has all the benchmarks and charts used in the paper.

Results land as `bench_*.csv` / `example_*.csv` (one row per run:
backend, timings, worker/chunk columns), ready for pandas/matplotlib
analysis in the paper.

## Disclaimer

> "The Vulkan backend architecture, AST flattening strategy, VRAM-aware batch sizing, and pipeline design were designed by the author. AI tooling was used to assist with implementation of low-level Vulkan API boilerplate."
