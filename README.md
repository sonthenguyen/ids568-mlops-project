# IDS568 MLOps Environment Setup

![CI](https://github.com/sonthenguyen/ids568-mlops-project/actions/workflows/ci.yml/badge.svg)

## Setup
This repository uses a pinned Python environment to ensure reproducible results.

### Requirements
- Python 3.12

### Create and activate environment
```bash
python -m venv .venv
source .venv/Scripts/activate
pip install -r requirements.txt

### Documentation
Environment reproducibility is essential for reliable machine learning systems across the full lifecycle, from data preparation to deployment. If Python or library versions differ between environments, the same code can behave inconsistently or fail. This repository addresses that risk by using an isolated Python virtual environment and pinning exact dependency versions in requirements.txt, which defines a clear and reproducible setup.

A minimal smoke test validates that required dependencies can be imported, and GitHub Actions runs this test automatically in a clean environment on every push and pull request. This automated validation ensures the environment can be recreated from scratch and works outside the original machine. By enforcing consistency between development and deployment environments, this setup prevents common reproducibility issues and provides a stable foundation for future ML pipeline and model deployment work.

