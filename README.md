# AI Academy - Machine Learning 101

[![GitHub](https://img.shields.io/badge/--181717?logo=github&logoColor=ffffff)](https://github.com/)
[Cloud2BR TEC](https://github.com/Cloud2BR-TEC)

Last updated: 2026-07-13

----------

Level 101 is the foundational entry point of the Machine Learning academy path.

This repository uses the GitHub Pages layout from the advanced Azure ML training site and reorganizes the content for a beginner-first learning flow. It consolidates the source material from:

- Azure-ML-Overview
- Azure-ML-Advanced

## Learning Path Strategy

The full academy is structured as three levels:

- Level 101: Fundamentals, Azure ML workspace basics, first model build, first deployment, and IaC introduction.
- Level 102: Intermediate engineering practices, reusable pipelines, monitoring strategy, and stronger MLOps controls.
- Level 103: Advanced production operations, governance, reliability, and enterprise-scale deployment patterns.

This repository currently publishes Level 101.

## Local Preview

```bash
pip install mkdocs mkdocs-material mkdocs-mermaid2-plugin pymdown-extensions
mkdocs serve
```

## Build for GitHub Pages

```bash
mkdocs build --strict
```

GitHub Pages deployment is configured in [.github/workflows/deploy-github-pages.yml](.github/workflows/deploy-github-pages.yml).

In GitHub repository settings, set:

- Settings -> Pages -> Source = GitHub Actions
