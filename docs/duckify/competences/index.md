# Compétences

Démonstrations des compétences demandées lors du projet **Duckify**.

---

## Analyser un problème informatique complexe

J'ai analysé le problème de la projection de texture sur modèle 3D -> [rapport d'analyse de projection](https://toys-r-us-rex.github.io/Duckify/research/projection_solution.pdf)

J'ai analyés les problèmes de `small artefacts` - `color quantization` - `Fill slicing` liées au pipeline de tracing établit originellement -> [rapport d'analyse du pipeline](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)

J'ai analysé le problème du nombres du points par traces trop élevé -> [rapport d'analyse](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/reduction.pdf)

J'ai analysé le problème issue de l'implémentation de la réduction du nombre de points par trace -> [rapport de debug](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/fill-slicing-debug-2.pdf)

J'ai identifié la source de traces sautant d'un bloc à l'autre de la UV map -> [rapport d'analyse](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/uv-map-correction.pdf)

J'ai identifié la source de la non-détection des bords imbriqués -> [rapport d'analyse](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/border-detection-refinement.pdf)

---

## Concevoir une solution théorique modélisée

J'ai participé à la conception globale du pipeline de tracing -> [plan de conception globale](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/general-overview.pdf)

J'ai participé à la conception technique détaillée du pipeline de tracing -> [plan de conception détaillée](https://toys-r-us-rex.github.io/Duckify/architecture/tracing_algo.pdf)

J'ai participé à la révision du pipeline de tracing et ai conçu une solution aux problèmes de  `small artefacts` - `color quantization` - `Fill slicing` -> [plan de la révision](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)

J'ai conçu deux approches complémentaires pour le problème de la réduction de points -> [rapport d'analyse](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/reduction.pdf)

J'ai conçu un correctif au problème des traces sautant d'un bloc à l'autre de la UV map -> [rapport de debug](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/uv-map-correction.pdf)

J'ai conçu une solution à la récupération des bords de contours imbriqués -> [rapport d'analyse](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/border-detection-refinement.pdf)

---

## Implémenter une approche théorique modélisée

J'ai implémenté des méthodes du pipeline de tracing `Tracer` (`load_texture`, `load_model`, `palettize_texture`, `split_colors`, `compute_fill_slices`, `format_palette`) -> [code source](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py)

J'ai implémenté la détection des contours imbriqués -> [PR #42 (nested border retrieval)](https://github.com/Toys-R-Us-Rex/Duckify/pull/42)

J'ai implémenté des correctifs au pipeline de tracing concernant les problèmes de `small artefacts` - `color quantization` - `Fill slicing` -> [PR #74 (small artefacts & fill slicing)](https://github.com/Toys-R-Us-Rex/Duckify/pull/74) + [PR #65 (color quantization)](https://github.com/Toys-R-Us-Rex/Duckify/pull/65)

J'ai rearrangé la disposition des blocs sur la UV map -> [PR #90 (UV map correction)](https://github.com/Toys-R-Us-Rex/Duckify/pull/90).

J'ai implémenter la réduction du nombre de points par trace -> [PR #92 (Reduce number of points in contours)](https://github.com/Toys-R-Us-Rex/Duckify/pull/92) 

J'ai corrigé le bug résultant de l'implémentation de la réduction du nombre de points par trace ->  [PR #96 (fill slicing debug 2)](https://github.com/Toys-R-Us-Rex/Duckify/pull/96)

---

## Evaluer un système informatique

J'ai évalué le TEXTurePaper -> [rapport d'évaluation TEXTure](https://toys-r-us-rex.github.io/Duckify/research/projection_solution.pdf)

J'ai comparé deux algorithmes de palettisation (MEDIANCUT vs KNN ) -> [rapport de comparaison](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)

J'ai évalué et rejeté l'approche par blurring pour le problème de `small artefacts` -> [rapport de comparaison](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)

J'ai évalué et validé les corrections aux problèmes de `small artefacts` & `Fill slicing` -> [rapport de comparaison](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf) + [PR #74 (small artefacts & fill slicing)](https://github.com/Toys-R-Us-Rex/Duckify/pull/74)

J'ai évalué le pipeline `ur3e-control` de la team robot -> [rapport d'évaluation de `ur3e-control`](https://toys-r-us-rex.github.io/Duckify/architecture/robot/audit/2026-03-18.pdf)

J'ai évalué l'effet de la réduction du nombre de points par trace  -> [rapport d'analyse](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/reduction.pdf)

---

## Valoriser des ensembles de données hétérogènes et multimodales

J'ai contribué à la valorisation de textures 2D et modèles 3D à l'aide du pipeline de tracing -> [par exemple avec `palettize_texture()`, `split_colors()` dans tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py)

J'ai produit un datasets de traces `.json` exploitables par la team robot, à partie de Blender/GenAI generated textures et avec l'aide du pipeline de tracing -> [permalink du dataset](https://github.com/Toys-R-Us-Rex/Duckify/tree/225b5667aa85d8fd0943a80ceb476a10f64c6247/assets/tests)

---

## Orchestrer un processus et une infrastructure de traitement de données

J'ai participé à l'orchestraion d'un pipeline de tracing -> [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py)

J'ai sélectionné et justifié le choix de la méthode KNN pour la palettisation -> [rapport (The color quantization (palettization) problem)](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)

---

## Appliquer les compétences de l'ingénierie en informatique au domaine des données

J'ai appliqué les principes POO à la classe `Tracer`, encapsulation, paramétrage, configuration externalisée, pas de valeurs hardcodées -> [class Tracer](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py)

---

## Communiquer clairement et efficacement

J'ai rédigé des rapports des daily meetings avec une évolution de mon style vers du moins verbeux et vers la captation des commentaires -> [le 19.02.2026](https://toys-r-us-rex.github.io/Duckify/meetings/daily/2026-02-19.pdf), [le 03.03.2026](https://toys-r-us-rex.github.io/Duckify/meetings/daily/2026-03-03.pdf) et [le 25.03.2026](https://toys-r-us-rex.github.io/Duckify/meetings/daily/2026-03-25.pdf)

J'ai rédigé le procès-verbale de la réunion avec le client -> [pv-2026-02-26.pdf](https://toys-r-us-rex.github.io/Duckify/meetings/ceo/pv-2026-02-26.pdf)

J'ai rédigé le compte-rendu de la réunion de préparation de la présentation CEO -> [procès-verbal](https://toys-r-us-rex.github.io/Duckify/planning/demonstration_ceo.pdf)

J'ai rédigé plusieurs documents recensant des modifications du pipeline de tracing-> un [plan initial de mise à jour](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/artefacts-removal.pdf) jugé insuffisant puis un [plan révisé de mise à jour](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)

J'ai présenté mes contributions lors des meetings hebdomadaires avec le CTO -> [semaine 1](https://toys-r-us-rex.github.io/Duckify/presentations/20260220_duckify_meeting_week_1.pdf), [semaine 2](https://toys-r-us-rex.github.io/Duckify/presentations/20260227_duckify_meeting_week_2.pdf), [semaine 3](https://toys-r-us-rex.github.io/Duckify/presentations/20260306_duckify_meeting_week_3.pdf), [semaine 4](https://toys-r-us-rex.github.io/Duckify/presentations/20260313_duckify_meeting_week_4.pdf), [semaine 5](https://toys-r-us-rex.github.io/Duckify/presentations/20260320_duckify_meeting_week_5.pdf) et [semaine 6](https://toys-r-us-rex.github.io/Duckify/presentations/20260327_duckify_meeting_week_6.pdf)

J'ai formulé des demandes de changement lors de PRs -> [PR #68](https://github.com/Toys-R-Us-Rex/Duckify/pull/68), [PR #18](https://github.com/Toys-R-Us-Rex/Duckify/pull/18) et [PR #15](https://github.com/Toys-R-Us-Rex/Duckify/pull/15)

J'ai réalisé un montage vidéo pour le site du projet (impression 3d) -> [commit](https://github.com/Toys-R-Us-Rex/promotion-website/commit/8dc31319465fc11b26af4f02113c253841af5b52) / [vidéo](../../assets/accelerated_duck_3d_impression.mp4)

---

## Adopter une posture professionnelle facilitante face aux situations rencontrées

J'ai pris la parole en tant que chef du projet pour mettre sur la table un problème de retards récurrents -> [au fond du rapport du meeting](https://toys-r-us-rex.github.io/Duckify/meetings/daily/2026-03-12.pdf) + [preuve de chef de la semaine](https://toys-r-us-rex.github.io/Duckify/meetings/weekly/2026-03-06.pdf)

J'ai accepté positivement la critique de l'insuffisance de mon plan de mise à jour du pipeline venant de mon collègue et ai recommencé avec lui -> [plan initiale](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/artefacts-removal.pdf) vs [plan révisé](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf) / [PR #53 abandonnée](https://github.com/Toys-R-Us-Rex/Duckify/pull/53)

Je me suis adapté a un environement nouveau (robot) pour produire un document d'analyse de leur pipeline -> [posture décrite dans les hiring questions de la semaine 5](../journal/week5.md) + [rapport d'analyse](https://toys-r-us-rex.github.io/Duckify/architecture/robot/audit/2026-03-18.pdf)

J'ai pris en compte les remarques de PR review et ai implémenté les changements demandés -> [PR #7](https://github.com/Toys-R-Us-Rex/Duckify/pull/7), [PR #24](https://github.com/Toys-R-Us-Rex/Duckify/pull/24), [PR #32](https://github.com/Toys-R-Us-Rex/Duckify/pull/32), [PR #41](https://github.com/Toys-R-Us-Rex/Duckify/pull/41), [PR #42](https://github.com/Toys-R-Us-Rex/Duckify/pull/42), [PR #65](https://github.com/Toys-R-Us-Rex/Duckify/pull/65) et [PR #74](https://github.com/Toys-R-Us-Rex/Duckify/pull/74)

J'ai review des PRs contribuant ainsi a clôturer le travail de mes collègues pour faire avancer le projet -> [PR #2](https://github.com/Toys-R-Us-Rex/Duckify/pull/2), [PR #3](https://github.com/Toys-R-Us-Rex/Duckify/pull/3), [PR #14](https://github.com/Toys-R-Us-Rex/Duckify/pull/14), [PR #15](https://github.com/Toys-R-Us-Rex/Duckify/pull/15), [PR #17](https://github.com/Toys-R-Us-Rex/Duckify/pull/17), [PR #18](https://github.com/Toys-R-Us-Rex/Duckify/pull/18), [PR #20](https://github.com/Toys-R-Us-Rex/Duckify/pull/20), [PR #21](https://github.com/Toys-R-Us-Rex/Duckify/pull/21), [PR #22](https://github.com/Toys-R-Us-Rex/Duckify/pull/22), [PR #27](https://github.com/Toys-R-Us-Rex/Duckify/pull/27), [PR #33](https://github.com/Toys-R-Us-Rex/Duckify/pull/33), [PR #35](https://github.com/Toys-R-Us-Rex/Duckify/pull/35), [PR #39](https://github.com/Toys-R-Us-Rex/Duckify/pull/39), [PR #40](https://github.com/Toys-R-Us-Rex/Duckify/pull/40), [PR #50](https://github.com/Toys-R-Us-Rex/Duckify/pull/50), [PR #54](https://github.com/Toys-R-Us-Rex/Duckify/pull/54), [PR #55](https://github.com/Toys-R-Us-Rex/Duckify/pull/55), [PR #56](https://github.com/Toys-R-Us-Rex/Duckify/pull/56), [PR #59](https://github.com/Toys-R-Us-Rex/Duckify/pull/59), [PR #68](https://github.com/Toys-R-Us-Rex/Duckify/pull/68), [PR #72](https://github.com/Toys-R-Us-Rex/Duckify/pull/72), [PR #73](https://github.com/Toys-R-Us-Rex/Duckify/pull/73), [PR #86](https://github.com/Toys-R-Us-Rex/Duckify/pull/86), [PR #97](https://github.com/Toys-R-Us-Rex/Duckify/pull/97), [PR #101](https://github.com/Toys-R-Us-Rex/Duckify/pull/101), [PR #102](https://github.com/Toys-R-Us-Rex/Duckify/pull/102), [PR #106](https://github.com/Toys-R-Us-Rex/Duckify/pull/106),[PR #117](https://github.com/Toys-R-Us-Rex/Duckify/pull/117)

J'ai pris mes responsabilités en dignostiquant et corrigeant un bug issu de mon travail -> [PR #96 (fill slicing debug 2)](https://github.com/Toys-R-Us-Rex/Duckify/pull/96)

J'ai participé à la préparation de la présentation finale avec le client en collaboration inter-équipe  -> [rapport du meeting](https://toys-r-us-rex.github.io/Duckify/planning/demonstration_ceo.pdf)

---

## Argumenter ses opinions et ses choix lors de processus décisionnels et stratégiques

J'ai argumenté contre l'adoption de TEXTurePaper -> [rapport d'analyse de TEXTurePaper](https://toys-r-us-rex.github.io/Duckify/research/projection_solution.pdf)

J'ai argumenté le remplacement de MEDIANCUT par KNN -> [rapport d'analyse](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)

J'ai argumenté le rejet du blur comme solution au problème de `small artefacts` -> [rapport d'analyse](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)

J'ai argumenté l'impact des changements de la disposition de la UV map en réponse au questionnement d'un collègue -> [commentaires de la PR #90](https://github.com/Toys-R-Us-Rex/Duckify/pull/90)

J'ai postulé l'impact de la réduction du nombre de points par traces -> [rapport d'analyse](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/reduction.pdf)

J'ai justifié le choix des trois textures pour la présentation finale -> [rapport de meeting](https://toys-r-us-rex.github.io/Duckify/planning/demonstration_ceo.pdfnamettre)

---

## Critiquer le déroulement d'une production de manière auto-réflexive

J'ai formulé une critique du pipeline de tracing et de sa mise à jour-> [au fond du document](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/improvements.pdf)

J'ai apporté une critique de mon travail lors de présentations hebdomadaires au CTO -> [semaine 2 (slides 8 et 12)](https://toys-r-us-rex.github.io/Duckify/presentations/20260227_duckify_meeting_week_2.pdf), [semaine 3 (slide 11)](https://toys-r-us-rex.github.io/Duckify/presentations/20260306_duckify_meeting_week_3.pdf), [semaine 6 (slide 13 et 19)](https://toys-r-us-rex.github.io/Duckify/presentations/20260327_duckify_meeting_week_6.pdf)

J'ai rédigé dans ce portfolio mes self-reflections -> [semaine 1](../journal/week1.md), [semaine 2](../journal/week2.md), [semaine 3](../journal/week3.md), [semaine 4](../journal/week4.md), [semaine 5](../journal/week5.md) et [semaine 6](../journal/week6.md)

J'ai formulé une critique de la réduction de points par trace -> [rapport d'analyse](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/reduction.pdf)

J'ai formulé une critique de mon implémentation de la réduction du nombre de points par traces et de ses conséquences -> [rapport de debug](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/fill-slicing-debug-2.pdf)

J'ai formulé une critique sur mon processus de résolution du problème de la UV map -> [rapport de debug](https://toys-r-us-rex.github.io/Duckify/architecture/tracing/uv-map-correction.pdf)
