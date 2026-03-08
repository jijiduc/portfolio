# Leverage heterogeneous and multimodal datasets

Statistically analyse data properties, advise on appropriate data collection, clean and prepare heterogeneous data from different domains (images, texts, signals, etc.), and assess the quality and overall value of datasets.

---

??? example "W2 · Texture palettization and color splitting"
    **Action:** Implemented `palettize_texture()` and `split_colors()` in the `Tracer` class.

    **Artifact:** [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py)

    **Justification:** These methods process raw image data (textures) and 3D model data simultaneously. Palettizing reduces the color space to a the disered palette and splitting then decomposes into exploitable color segments.

    **Reference:** [Week 2](../../journal/week2.md)
