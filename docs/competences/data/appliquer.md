# Apply CS engineering skills to the data domain

Integrate sensor data into a perception → decision → action loop with a robust software architecture (tests, integration, deployment), or design a software chain that transforms multimodal data into exploitable indicators while ensuring system integration, security, and traceability.

---

??? example "W2 · Tracer class implementation"
    **Action:** Implemented the `Tracer` class as part of the tracing pipeline.

    **Artifact:** [tracer.py](https://github.com/Toys-R-Us-Rex/Duckify/blob/ea67d8677b94415608ee8e75b3b0258242b4d44f/tracing/tracer.py)

    **Justification:** The `Tracer` class applies OOP principles to a data processing problem.

    **Reference:** [Week 2](../../journal/week2.md)

??? example "W3 · detect_islands() update"
    **Action:** Updated `detect_islands()` and the relevant parts of the `Tracer` class to support multi-layer border detection.

    **Artifact:** [PR #42](https://github.com/Toys-R-Us-Rex/Duckify/pull/42/commits)

    **Justification:** This function extension requiered understanding of the pipeline and was designed with modularity in mind (Class Hierarchy new methods).

    **Reference:** [Week 3](../../journal/week3.md)
