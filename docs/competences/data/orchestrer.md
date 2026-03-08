# Orchestrate a data processing pipeline and infrastructure

Develop a complete data processing pipeline (collection, cleaning, training, deployment), select adequate and justified methods (statistical analysis, computational modelling, numerical simulation, or machine learning), and produce a discriminative, predictive, or generative software solution.

---

??? example "W2 · Tracing pipeline orchestration"
    **Action:** Implemented the core orchestration methods of the `Tracer` class.

    **Artifact:** [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py)

    **Methods implemented:**

    - `load_texture()` — ingests texture input
    - `load_model()` — ingests 3D model input
    - `compute_fill_slices()` — computes intermediate processing steps
    - `format_palette()` — formats final output

    **Justification:** These methods collectively form the data pipeline: ingest → process → output. Each step is explicitly ordered and feeds into the next, which is the definition of pipeline orchestration.

    **Reference:** [Week 2](../../journal/week2.md)
