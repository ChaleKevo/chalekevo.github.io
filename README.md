# Kevin Magoma — Research Portfolio

[![ORCID](https://img.shields.io/badge/ORCID-0009--0009--3298--7130-green.svg)](https://orcid.org/0009-0009-3298-7130)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23840592.svg)](https://doi.org/10.5281/zenodo.23840592)
[![Website](https://img.shields.io/badge/Portfolio-Live_Site-blue.svg)](https://chalekevo.github.io/kevinmagoma.github.io/)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

Academic repository and research portfolio for **Kevin Magoma**, focusing on AI systems, token economics, and execution latency profiling across autonomous multi-agent software engineering pipelines.

---

## 🔬 Research Overview

Modern code generation systems increasingly decompose tasks into specialized sub-agents (e.g., planners, coders, unit-test generators, and critics). While role decomposition mitigates error cascades in non-trivial systems tasks, it introduces substantial computational latency and token expansion overhead.

My research focuses on:
* **Inference Economics & Token Scalability:** Characterizing cumulative context expansion, memory decay, and redundant computation across autonomous agent loops.
* **Execution Latency Profiling:** Benchmarking end-to-end convergence rates across monolithic zero-shot pipelines versus decomposed agent consensus workflows.
* **Adaptive Sub-Agent Task Routing:** Designing heuristic metrics (based on cyclomatic complexity and dependency graphs) that determine whether a programming task warrants multi-agent decomposition or direct single-pass synthesis.

---

## 📄 Publications & Technical Reports

### [Empirical Analysis of Token Consumption and Execution Latency in Multi-Agent Code Generation Pipelines](https://doi.org/10.5281/zenodo.23840592)
* **Author:** Kevin Magoma
* **Type:** Technical Note / Research Report
* **Published:** October 2025
* **Permanent DOI:** [`10.5281/zenodo.23840592`](https://doi.org/10.5281/zenodo.23840592)
* **Access:** Open Access (CC-BY 4.0)

**Abstract:**  
Recent advancements in large language models (LLMs) have shifted automated programming from single-prompt generation to multi-agent architectures where agents divide tasks across planning, implementation, and test validation. While these architectures demonstrate superior pass rates on complex benchmarks, their computational overhead remains poorly characterized in production settings. This paper evaluates the operational trade-offs between monolithic agent pipelines and decomposed multi-agent networks across 50 algorithmic and systems-level programming tasks. We analyze token consumption patterns, wall-clock latency, and repair efficiency across automated iterations. Our findings reveal that while decomposed multi-agent frameworks yield a 24% relative reduction in logical syntax regressions, they incur a 3.1x expansion in cumulative token usage. We propose an adaptive task routing metric that predicts optimal architectural decomposition based on initial dependency complexity.

```bibtex
@techreport{magoma2025empirical,
  title       = {Empirical Analysis of Token Consumption and Execution Latency in Multi-Agent Code Generation Pipelines},
  author      = {Magoma, Kevin},
  year        = {2025},
  month       = {October},
  institution = {Zenodo},
  doi         = {10.5281/zenodo.23840592},
  url         = {https://doi.org/10.5281/zenodo.23840592}
}
```

---

## 🛠️ Active Projects & Tooling

### Adaptive Sub-Agent Dispatch Engine
An experimental evaluation harness that parses abstract syntax trees (ASTs) of incoming programming tickets to calculate dependency depth and branch complexity. 
* Lightweight functions ($\theta < 0.35$) route directly to monolithic single-pass generation, conserving up to 65% in token expenditure.
* High-cyclomatic modules ($\theta \ge 0.35$) automatically engage role-decomposed multi-agent consensus loops with contract validation.

### Benchmark Infrastructure & Evaluation Stack
* **Runtime Profiling:** Python 3.11+, PyTorch, vLLM
* **Sandboxing & Isolation:** Docker containers, Git worktrees
* **Analysis & Verification:** Abstract Syntax Tree (AST) parsing, Pytest tracing harnesses, Pandas

---

## 🪪 Academic Identifiers & Contact

| Record | Identifier / Link |
| :--- | :--- |
| **ORCID** | [0009-0009-3298-7130](https://orcid.org/0009-0009-3298-7130) |
| **Permanent DOI** | [10.5281/zenodo.23840592](https://doi.org/10.5281/zenodo.23840592) |
| **Live Portfolio** | [chalekevo.github.io/kevinmagoma.github.io](https://chalekevo.github.io/kevinmagoma.github.io/) |
| **Contact Email** | [chalekevo@gmail.com](mailto:chalekevo@gmail.com) |

---

*© 2025 Kevin Magoma. Open science and reproducible research.*
