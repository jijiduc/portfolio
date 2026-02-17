# Duc Jeremy // Engineering Portfolio & Knowledge Base

![CI/CD Status](https://github.com/jijiduc/portfolio/actions/workflows/ci.yml/badge.svg)
![Python Version](https://img.shields.io/badge/python-3.8%2B-blue)
![MkDocs](https://img.shields.io/badge/built%20with-MkDocs-green)

Ce dépôt contient le code source et la documentation technique de mon portfolio personnel.
Le site est généré statiquement via **MkDocs** avec le thème **Material**, hébergé sur GitHub Pages.

🔗 **Version Live :** [https://jijiduc.github.io/portfolio/]

## Architecture

Ce projet suit l'approche **Docs as Code**.
- **Moteur :** MkDocs (Python)
- **Thème :** Material for MkDocs
- **Maths :** MathJax & LaTeX support
- **Déploiement :** GitHub Actions (CI/CD)

## Installation Locale

Pour prévisualiser le site ou contribuer à la documentation :

### 1. Prérequis
- Python 3.8 ou supérieur
- Git

### 2. Initialisation
```bash
# Cloner le dépôt
git clone https://github.com/jijiduc/portfolio.git
cd portfolio

# Créer un environnement virtuel (Recommandé)
python -m venv venv
venv\Scripts\activate

# Installer les dépendances
pip install mkdocs-material

### 3. Lancer le serveur de développement
mkdocs serve
```
Le site sera accessible à [l'adresse suivante](http://127.0.0.1:8000/).

## Déploiement
Le déploiement est entièrement automatisé.
Tout push sur la branche main déclenche le workflow GitHub Actions défini dans `.github/workflows/ci.yml`, qui compile le Markdown en HTML et le publie sur la branche `gh-pages`.
