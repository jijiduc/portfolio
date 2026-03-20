# Compétences

Recensement des démonstrations des compétences demandées lors du projet **Duckify**.

---

## Analyser un problème informatique complexe

J'ai recherché des solutions existantes pour la problématique de la projection de texture sur modèle 3D. Le [rapport](https://toys-r-us-rex.github.io/Duckify/research/projection_solution.pdf) en résultant démontre ce travail.


J'ai participé à la rédaction d'un plan structurant les modifications à apporter au pipeline de Tracing établit. Le [plan](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf) démontre ma capacité à identifier les problèmes du pipeline et en apporter des solutions. Par exemple, que l'algorithme MEDIANCUT biaisait la palette en faveur de la couleur dominante (le noir du masque UV).

---

## Concevoir une solution théorique modélisée

J'ai participé à la conception du pipeline de tracing en définissant pour chaque étape les entrées/sorties et leur enchaînement. Le [document](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/general-overview.pdf) recense cette modélisation.

---

## Implémenter une approche théorique modélisée

J'ai implémenté six méthodes de la classe `Tracer` (`load_texture`, `load_model`, `palettize_texture`, `split_colors`, `compute_fill_slices`, `format_palette`) conformément à l'architecture prédéfinie. Le fichier du code implémenté, [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py). démontre ma capacité à transposer d'un modèle théorique à l'implémentation.

---

## Evaluer un système informatique

J'ai évalué TEXTurePaper comme potentielle solution à l'étape de projection de texture. La conclusion du [rapport](https://toys-r-us-rex.github.io/Duckify/research/projection_solution.pdf) démontre les résultats de mon évaluation.

J'ai comparé deux algorithmes de palettisation et établi que MEDIANCUT produit une palette biaisée par la couleur dominante, tandis que KNN garantit un poids égal à chaque couleur et supporte un paramètre d'exclusion. Cette évaluation, formalisée dans le [document](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf), c'est transcrite en une mise à jour du pipeline.

---

## Valoriser des ensembles de données hétérogènes et multimodales

J'ai implémenté les méthodes`palettize_texture()` et `split_colors()` dans la classe `Tracer`. Le fichier [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py) contenant la classe, démontre le traitement des données mis en place (image texture et modèle 3D) aboutissant à la réduction de l'espace colorimétrique vers la palette souhaitée et la décomposition de la texture en couche de couleur.


---

## Orchestrer un processus et une infrastructure de traitement de données

J'ai implémenté les méthodes d'orchestration de la classe `Tracer` (`load_texture`, `load_model`, `compute_fill_slices`, `format_palette`), formant une partie du pipeline complet. Le fichier [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py) démontre cette structuration du flux de données.

---

## Appliquer les compétences de l'ingénierie en informatique au domaine des données

J'ai participé à la conception et l'implémentation de la classe `Tracer` en y appliquant les principes de la programmation orientée objet. Le fichier [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py) démontre l'utilisation de bonnes pratiques d'ingénierie (encapsulation, aucune de valeurs hardcodées, fichier de configuration) à un pipeline de données.


---

## Communiquer clairement et efficacement


J'ai rédigé les comptes-rendus des daily meeting du [19.02.2026](https://toys-r-us-rex.github.io/Duckify/meetings/daily/2026-02-19.pdf) et du [03.03.2026](https://toys-r-us-rex.github.io/Duckify/meetings/daily/2026-03-03.pdf). Dans le second rapport, j'utilise un style plus concis afin d'éviter de surcharger le rapport.

J'ai rédigé le procès-verbale de la réunion avec le client [pv-2026-02-26.pdf](https://toys-r-us-rex.github.io/Duckify/meetings/ceo/pv-2026-02-26.pdf). Ce document démontre ma capacité à synthétiser de manière constreinte le déroulé et les décisions du meeting.

J'ai rédigé deux documents de planification technique lors de mise à jour du pipeline de tracing: un [plan initial](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/artefacts-removal.pdf) puis un [plan révisé](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)(rédigé avec Louis) après intégration de son retour. L'évolution du style montre une progression vers un style moins verbeux et plus technique.

À la fin de chaque semaine, j'ai présenté mon travail au sein de la team tracing en exposant les avancées, les blockers rencontrés et les résolutions adoptées. Les présentations des [semaines 2](https://toys-r-us-rex.github.io/Duckify/presentations/20260227_duckify_meeting_week_2.pdf), [3](https://toys-r-us-rex.github.io/Duckify/presentations/20260306_duckify_meeting_week_3.pdf) et [4](https://toys-r-us-rex.github.io/Duckify/presentations/20260313_duckify_meeting_week_4.pdf) démontrent ma capacité à prendre du recul sur mon travail à identifier les éléments blockers.

---

## Adopter une posture professionnelle facilitante face aux situations rencontrées

Face à un problème de retards récurrents lors des daily meeting, j'ai pris la parole pour pointer le problème et proposé des alternatives à la forme actuelle. Au fond du [rapport du meeting](https://toys-r-us-rex.github.io/Duckify/meetings/daily/2026-03-12.pdf), cette intervention est recensée.

Face à un premier plan jugé insuffisant par mon collègue Louis, j'ai accepté positivement la critique et recommencé ce travail avec lui. Le [plan révisé](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf) démontre ce changement et ma capacité à prendre une posture professionelle face à un déconvenu sentimental.

---

## Argumenter ses opinions et ses choix lors de processus décisionnels et stratégiques

J'ai argumenté contre l'adoption de TEXTurePaper en structurant mon analyse autour de critères objectifs : format de sortie inadapté, dépendances inclaire, modèle hébergé disparu. Le rapport [projection_solution.pdf](https://toys-r-us-rex.github.io/Duckify/research/projection_solution.pdf) contient mon argumentaire.

J'ai argumenté le remplacement de MEDIANCUT par KNN en m'appuyant sur des faits techniques mesurables : biais par la couleur dominante, absence de paramètre d'exclusion, distribution déséquilibrée de la palette. L'argument est formalisé dans le [rapport](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf).

---

## Critiquer le déroulement d'une production de manière auto-réflexive

À la fin de chaque semaine, j'ai présenté mon travail au sein de la team tracing en exposant les avancées, les blockers rencontrés et les résolutions adoptées. Les présentations des [semaines 2](https://toys-r-us-rex.github.io/Duckify/presentations/20260227_duckify_meeting_week_2.pdf), [3](https://toys-r-us-rex.github.io/Duckify/presentations/20260306_duckify_meeting_week_3.pdf) et [4](https://toys-r-us-rex.github.io/Duckify/presentations/20260313_duckify_meeting_week_4.pdf) démontrent ma capacité à prendre du recul sur mon travail à identifier les éléments blockers.

Chaque semaine, j'ai rédigé dans ce portfolio une section de self-reflection expliquant ce qui s'est bien passé, ce qui pourrait être amélioré et ce qui a été appris. Ces entrées des [semaines 1](../journal/week1.md), [2](../journal/week2.md), [3](../journal/week3.md) et [4](../journal/week4.md) constituent une trace écrite de ma capacité à m'analyser et à en tirer des leçons.

