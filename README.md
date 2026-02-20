# Duc Jeremy // Engineering Portfolio & Knowledge Base

![CI/CD Status](https://github.com/jijiduc/portfolio/actions/workflows/ci.yml/badge.svg)
![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![MkDocs](https://img.shields.io/badge/built%20with-MkDocs-green)

This repository contains the source code and technical documentation for my personal portfolio.
The site is statically generated via **MkDocs** with the **Material** theme, hosted on GitHub Pages.

🔗 **Live Version:** [https://jijiduc.github.io/portfolio/]

## Architecture

This project follows the **Docs as Code** approach.
- **Engine:** MkDocs (Python)
- **Theme:** Material for MkDocs
- **Math:** MathJax & LaTeX support
- **Deployment:** GitHub Actions (CI/CD)

## Local Installation

To preview the site or contribute to the documentation:

### 1. Prerequisites
- Python 3.8 or higher
- Git

### 2. Initialization
```bash
# Clone the repository
git clone https://github.com/jijiduc/portfolio.git
cd portfolio

# Create a virtual environment (Recommended)
python -m venv venv
venv\Scripts\activate

# Install dependencies
pip install mkdocs-material

### 3. Run the development server
mkdocs serve
```
The site will be accessible at [the following address](http://127.0.0.1:8000/).

## Deployment
Deployment is fully automated.
Every push to the main branch triggers the GitHub Actions workflow defined in `.github/workflows/ci.yml`, which compiles Markdown into HTML and publishes it to the `gh-pages` branch.
