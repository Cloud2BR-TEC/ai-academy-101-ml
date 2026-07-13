# Machine Learning 101 Course

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR TEC](https://github.com/Cloud2BR-TEC)

Last updated: 2026-07-13

----------

Course 101 is a foundational machine learning course focused on practical Azure ML basics.

This repository uses the GitHub Pages layout from the advanced Azure ML training site and reorganizes the content for a beginner-first learning flow. It consolidates the source material from:

- Azure-ML-Overview
- Azure-ML-Advanced

## Course Scope

This repository publishes only Course 101 content:

- Machine learning basics for beginners.
- Azure ML workspace and lifecycle fundamentals.
- First model training, evaluation, and deployment.
- Introductory infrastructure as code with Terraform.

## Local Preview

```bash
pip install mkdocs mkdocs-material pymdown-extensions
mkdocs serve
```

## Build for GitHub Pages

```bash
mkdocs build --strict
```

GitHub Pages deployment is configured in [.github/workflows/deploy-github-pages.yml](.github/workflows/deploy-github-pages.yml).

In GitHub repository settings, set:

- Settings -> Pages -> Source = GitHub Actions
