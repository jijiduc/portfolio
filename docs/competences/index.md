# Compétences

Recensement des démonstrations des compétences demandées lors du projet **Duckify**.

---

## Analyser un problème informatique complexe

J'ai recherché des solutions existantes pour la problématique de la projection de texture sur modèle 3D. Le [rapport](https://toys-r-us-rex.github.io/Duckify/research/projection_solution.pdf) en résultant démontre ce travail.

J'ai participé à la rédaction d'un plan structurant les modifications à apporter au pipeline de Tracing établit. Le [plan](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf) démontre ma capacité à identifier les problèmes du pipeline et en apporter des solutions. Par exemple, que l'algorithme MEDIANCUT biaisait la palette en faveur de la couleur dominante (le noir du masque UV).

---

## Concevoir une solution théorique modélisée

J'ai participé à la conception du pipeline de tracing en définissant pour chaque étape les entrées/sorties et leur enchaînement. Le problème est pluridisciplinaire : il croise la géométrie 3D (UV maps, mesh), le traitement d'image (espace colorimétrique, texture) et les contraintes robotiques (taille minimale des îlots traçables, nombre de points par contour). Le [document](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/general-overview.pdf) recense cette modélisation initiale.

J'ai participé à la révision du pipeline après identification de modifications à faire comme le biais de palettisation ou la présence det petits artefacts. Le [plan révisé](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf) présente cette modélisation, démontrant ma capacité à faire évoluer un modèle et a rechercher et justifier les changements.

---

## Implémenter une approche théorique modélisée

J'ai implémenté six méthodes de la classe `Tracer` (`load_texture`, `load_model`, `palettize_texture`, `split_colors`, `compute_fill_slices`, `format_palette`) conformément à l'architecture prédéfinie. Le fichier du code implémenté, [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py), démontre ma capacité à transposer d'un modèle théorique à l'implémentation.

J'ai corrigé les bugs de fill slicing et ai enlevés les artefacts de couleur indésirables afin d'éviter que le pipeline ne génère des îlots trop petits/non traçables avec les feutres. Ces corrections sont explicitées dans la [PR #74](https://github.com/Toys-R-Us-Rex/Duckify/pull/74).

J'ai remappé la disposition des UV du modèle canard pour garantir une séparation suffisante entre les blocs UV, conformément aux contraintes du pipeline de tracing. Cette modification est disponible dans la [PR #90](https://github.com/Toys-R-Us-Rex/Duckify/pull/90).

J'ai réduit le nombre de points par trace à la demande de la team robot. Cette modification est explicite dans la [PR #92](https://github.com/Toys-R-Us-Rex/Duckify/pull/92), et la correction du bug résultant dans la [PR #96](https://github.com/Toys-R-Us-Rex/Duckify/pull/96).

---

## Evaluer un système informatique

J'ai évalué TEXTurePaper comme potentielle solution à l'étape de projection de texture. La conclusion du [rapport](https://toys-r-us-rex.github.io/Duckify/research/projection_solution.pdf) démontre les résultats de mon évaluation.

J'ai comparé deux algorithmes de palettisation et établi que MEDIANCUT produit une palette biaisée par la couleur dominante, tandis que KNN garantit un poids égal à chaque couleur et supporte un paramètre d'exclusion. Cette évaluation, disponible dans le [document](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf), s'est ensuite transcrite en une mise à jour du pipeline.

J'ai évalué le pipeline `ur3e-control` de la team robot en tant qu' externe. Le [rapport](https://toys-r-us-rex.github.io/Duckify/architecture/robot/audit/2026-03-18.pdf) démontre ma capacité d'évaluation dans un environnement nouveau.

---

## Valoriser des ensembles de données hétérogènes et multimodales

J'ai conçu le traitement combinant une image de texture (2D) et un modèle 3D pour réduire l'espace colorimétrique vers une palette cible et décomposer la texture en couches par couleur. Les méthodes `palettize_texture()` et `split_colors()` dans [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py) montrent comment ces deux types de données hétérogènes sont mis en correspondance pour produire une représentation colorimétrique structurée et exploitable.

J'ai utilisé Blender + pipeline de tracing → fichiers de sortie pour produire des datasets de traces utilisables par la team robot. ce faisant, valorisant les données dans le pipeline. Le résultat est disponible dans les [PR #82](https://github.com/Toys-R-Us-Rex/Duckify/pull/82) et [PR #99](https://github.com/Toys-R-Us-Rex/Duckify/pull/99), et démontrent ma capacité a valoriser des données.
---

## Orchestrer un processus et une infrastructure de traitement de données

J'ai structuré le pipeline de tracing au sein de la classe `Tracer` en définissant le flux de données d'entrées (texture, modèle) à aux sorties (palettes, slices). Le fichier [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py) démontre cette organisation du flux via les méthodes `load_texture`, `load_model`, `compute_fill_slices` et `format_palette`.

J'ai sélectionné la méthode KNN pour la mise à jour de la palettization en justifiant dans le [document suivant](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf). Ceci reflète ma capacité a sélectionné une méthode adéquate et à le justifier.

---

## Appliquer les compétences de l'ingénierie en informatique au domaine des données

J'ai appliqué les principes de la programmation orientée objet — encapsulation, paramétrage des variables, absence de valeurs hardcodées, fichier de configuration — à la classe `Tracer`. Le fichier [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py) illustre ces bonnes pratiques d'ingénierie appliquées à un pipeline de données.

---

## Communiquer clairement et efficacement

J'ai rédigé les comptes-rendus des daily meeting du [19.02.2026](https://toys-r-us-rex.github.io/Duckify/meetings/daily/2026-02-19.pdf), du [03.03.2026](https://toys-r-us-rex.github.io/Duckify/meetings/daily/2026-03-03.pdf) et du [25.03.2026](https://toys-r-us-rex.github.io/Duckify/meetings/daily/2026-03-25.pdf). Le second adopte un style plus concis pour éviter de surcharger le rapport. Le troisième démontre un effort sur la captation des échanges annexes au sujet principal, afin de retranscrire les discussions relevantes.

J'ai rédigé le procès-verbale de la réunion avec le client [pv-2026-02-26.pdf](https://toys-r-us-rex.github.io/Duckify/meetings/ceo/pv-2026-02-26.pdf). Ce document démontre ma capacité à synthétiser de manière constreinte le déroulé et les décisions du meeting.

J'ai rédigé deux documents de planification technique lors de mise à jour du pipeline de tracing: un [plan initial](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/artefacts-removal.pdf) puis un [plan révisé](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)(rédigé avec Louis) après intégration de son retour. L'évolution du style montre une progression vers un style moins verbeux et plus technique.

À la fin de chaque semaine, j'ai présenté mon travail au sein de la team tracing en exposant les avancées, les blockers rencontrés et les résolutions adoptées. Les présentations des [semaines 2](https://toys-r-us-rex.github.io/Duckify/presentations/20260227_duckify_meeting_week_2.pdf), [3](https://toys-r-us-rex.github.io/Duckify/presentations/20260306_duckify_meeting_week_3.pdf), [4](https://toys-r-us-rex.github.io/Duckify/presentations/20260313_duckify_meeting_week_4.pdf) et [5](https://toys-r-us-rex.github.io/Duckify/presentations/20200320_duckify_meeting_week_5.pdf) démontrent ma capacité à prendre du recul sur mon travail et à identifier les éléments blockers.

---

## Adopter une posture professionnelle facilitante face aux situations rencontrées

Face à un problème de retards récurrents lors des daily meeting, j'ai pris la parole, en tant que chef de la semaine, pour le pointer et proposer des alternatives au fonctionnement actuel. Au fond du [rapport du meeting](https://toys-r-us-rex.github.io/Duckify/meetings/daily/2026-03-12.pdf), cette intervention est recensée et mon rôle de chef de la semaine est notifié.

Face à un premier plan établit, jugé insuffisant par mon collègue Louis, j'ai accepté positivement la critique et recommencé ce travail avec lui. Le [plan révisé](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf) démontre ce changement et ma capacité à garder une posture professionelle face à un avis contraire.

Sollicité pour intervenir dans la team robot en tant qu'externe, je me suis adapté a un environement différent. J'ai d'abord pris contact avec les membres de l'équipe pour clarifier les attentes, puis ai parcouru le pipeline de manière autonome tout en sollicitant de l'aide sur les points à clarifer. Cette capacité d'adaptation à un contexte inconnu est relatée dans les [hiring questions de la semaine 5](../journal/week5.md) et le [rapport](https://toys-r-us-rex.github.io/Duckify/architecture/robot/audit/2026-03-18.pdf) prouve l'existence de ce travail.

---

## Argumenter ses opinions et ses choix lors de processus décisionnels et stratégiques

J'ai argumenté contre l'adoption de TEXTurePaper en structurant mon analyse autour de critères objectifs : format de sortie inadapté, dépendances inclaire, modèle hébergé disparu. Le rapport [projection_solution.pdf](https://toys-r-us-rex.github.io/Duckify/research/projection_solution.pdf) contient mon argumentaire.

J'ai argumenté le remplacement de MEDIANCUT par KNN en m'appuyant sur des faits techniques mesurables : biais par la couleur dominante, absence de paramètre d'exclusion, distribution déséquilibrée de la palette. L'argument est formalisé dans le [rapport](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf).

---

## Critiquer le déroulement d'une production de manière auto-réflexive

À la fin de chaque semaine, j'ai présenté mon travail au sein de la team tracing en exposant les avancées, les blockers rencontrés et les résolutions adoptées. Les présentations des [semaines 2](https://toys-r-us-rex.github.io/Duckify/presentations/20260227_duckify_meeting_week_2.pdf), [3](https://toys-r-us-rex.github.io/Duckify/presentations/20260306_duckify_meeting_week_3.pdf), [4](https://toys-r-us-rex.github.io/Duckify/presentations/20260313_duckify_meeting_week_4.pdf) et [5](https://toys-r-us-rex.github.io/Duckify/presentations/20200320_duckify_meeting_week_5.pdf) démontrent ma capacité à prendre du recul sur mon travail et à identifier les éléments blockers.

Chaque semaine, j'ai rédigé dans ce portfolio une section de self-reflection expliquant ce qui s'est bien passé, ce qui pourrait être amélioré et ce qui a été appris. Les entrées des [semaines 1](../journal/week1.md), [2](../journal/week2.md), [3](../journal/week3.md), [4](../journal/week4.md), [5](../journal/week5.md) et [6](../journal/week6.md) constituent une trace écrite de ma capacité à m'auto-analyser et à en tirer des leçons.
