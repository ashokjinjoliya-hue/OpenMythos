# Contributing to OpenMythos

Thank you for your interest in contributing! OpenMythos is a community-driven theoretical reconstruction — all contributions, from bug fixes to new architectural hypotheses, are welcome.

## Getting Started

```bash
git clone https://github.com/kyegomez/OpenMythos
cd OpenMythos
pip install -e ".[dev]"
```

## Development Workflow

1. **Fork** the repo and create a branch: `git checkout -b feat/your-feature`
2. **Make your changes** with tests where applicable
3. **Run lint**: `black . && ruff check .`
4. **Run tests**: `pytest tests/ test_main.py -v`
5. **Open a PR** against `main` with a clear description

## What We're Looking For

- Bug fixes and correctness improvements to the architecture
- New model variants or configuration presets
- Improved training scripts (multi-GPU, efficiency, etc.)
- Better documentation and usage examples
- Benchmark results comparing loop counts / model sizes

## Code Style

- **Black** for formatting (line length 88)
- **Ruff** for linting
- All new modules should have docstrings following the existing style

## Reporting Issues

Open a GitHub Issue with:
- Python and PyTorch versions
- Minimal reproducible example
- Full traceback

## Questions

Join the [Discord](https://discord.gg/EamjgSaEQf) for discussion.
