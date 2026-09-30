# Sample Project for CI/CD Reliability Testing

This project is intended to generate real GitHub Actions runs.

## Projects
- 01-simple-website: HTML + CSS
- 02-python-calculator: Python + pytest
- 03-flask-api: Flask + pytest

## Usage
Create a separate GitHub repository for each project, copy the files into it, and push to `main`.
The included `.github/workflows/ci.yml` workflow runs automatically.

## Generate failure data
For Python projects, temporarily change a test assertion so it fails, commit, and push.
For dependency testing, temporarily change a dependency to an invalid version, commit, and push.
Restore the working version afterward.

## Duplicate-code testing
Copy a function into another Python file and make small changes. This gives your duplicate-code detector realistic test input.
