# Contributing to Predictive Maintenance Arena

Thank you for your interest in contributing to the OCN ecosystem!

## Code of Conduct

All contributors are expected to uphold the [GALACTIC-UNION Code of Conduct](https://github.com/GALACTIC-UNION/.github/blob/main/CODE_OF_CONDUCT.md).

## How to Contribute

### 1. Fork and Clone

```bash
git clone https://github.com/<your-username>/predictive-maintenance-arena.git
cd predictive-maintenance-arena
git remote add upstream https://github.com/GALACTIC-UNION/predictive-maintenance-arena.git
```

### 2. Create a Branch

Use the naming convention: `feat/`, `fix/`, `docs/`, `test/`, or `chore/`.

```bash
git checkout -b feat/my-feature
```

### 3. Set Up the Development Environment

```bash
pip install -r config/requirements.txt
pip install -r config/requirements-dev.txt  # linting, testing extras
pre-commit install
```

### 4. Make Your Changes

- Write code in `src/` following the existing module structure.
- Add or update tests in `tests/` — aim for ≥ 90 % coverage on new code.
- Update `docs/` if your change affects public APIs or architecture.
- Follow [PEP 8](https://peps.python.org/pep-0008/) for Python code style.

### 5. Run Tests Locally

```bash
pytest tests/ -v --cov=src --cov-report=term-missing
flake8 src/ tests/
mypy src/
```

### 6. Commit with Conventional Commits

```
feat: add LSTM failure-prediction model
fix: correct sliding-window edge case in feature pipeline
docs: update architecture diagram
test: add integration tests for Kafka adapter
```

### 7. Open a Pull Request

- Push to your fork and open a PR against `main`.
- Fill in the PR template — describe the problem, solution, and testing done.
- A GALACTIC-UNION maintainer will review within 3 business days.
- CI must pass before merging.

## Reporting Issues

Use [GitHub Issues](https://github.com/GALACTIC-UNION/predictive-maintenance-arena/issues) with the appropriate label:
- `bug` — something is broken
- `enhancement` — new feature or improvement
- `documentation` — docs gap or error
- `question` — usage question

## Security Vulnerabilities

Do **not** open a public issue for security vulnerabilities. Email **security@galactic-union.io** instead.

## License

By contributing, you agree that your contributions will be licensed under the project's MIT License.
