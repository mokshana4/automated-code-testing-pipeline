# Automated Code Testing Pipeline

## Project Overview

This project demonstrates an automated Python testing pipeline using **pytest**, **Git**, **GitHub**, and **GitHub Actions**.

Whenever code changes are pushed to GitHub, GitHub Actions automatically installs the required dependencies and runs the automated tests.

## Technologies Used

- Python
- pytest
- Git and GitHub
- GitHub Actions
- YAML

## Project Structure

```text
automated-code-testing-pipeline/
├── .github/
│   └── workflows/
│       └── ci.yml
├── app.py
├── test_app.py
├── requirements.txt
└── README.md
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/mokshana4/automated-code-testing-pipeline.git
cd automated-code-testing-pipeline
```

### 2. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 3. Run the automated tests

```bash
python -m pytest -v
```

The tests verify the addition, subtraction, and multiplication functions in `app.py`.

## Continuous Integration

The GitHub Actions workflow is defined in `.github/workflows/ci.yml`.

The workflow automatically:

1. Checks out the repository.
2. Sets up Python.
3. Installs dependencies from `requirements.txt`.
4. Runs the pytest test suite.
5. Reports whether the workflow succeeds or fails.

## Learning Outcomes

- Writing automated unit tests with pytest.
- Managing Python dependencies.
- Tracking changes using Git.
- Hosting code on GitHub.
- Automating tests with GitHub Actions.
- Detecting failures and verifying fixes through CI.

## Future Improvements

- Add more unit tests and edge cases.
- Generate a test coverage report.
- Add code quality checks with a linter.
- Expand the pipeline with additional CI/CD stages.