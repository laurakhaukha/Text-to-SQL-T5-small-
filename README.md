#Schema-Augmented Prompt Engineering for Text-to-SQL Generation over SNOMED CT

This repository contains the full code, handcrafted dataset, and evaluation pipeline from my MSc Health Data Science dissertation. The project investigates whether schema-augmented prompt engineering can improve SQL generation for SNOMED CT using the lightweight T5-small model.

Key Components:

1. Schema-Augmented Prompting: Embeds the SNOMED CT schema (description & relationship tables) into prompts to guide SQL generation.

2. Few-Shot vs. Zero-Shot Comparison: Evaluates the impact of K=3 in-context examples per query category on executability and syntactic similarity.
   
3. Handcrafted NL–SQL Dataset: 120 balanced examples across six clinically motivated categories (e.g., concept lookups, synonym retrieval, hierarchical
   relationship exploration, aggregation queries).

4. Evaluation Framework: Includes Execution Accuracy (EA), Exact Match Accuracy (EMA), Average Sequence Match Score (ASMS), SQLGlot semantic equivalence, and
   Datacompy-based result set comparisons.

5. Error Analysis: Identifies key failure patterns, including directionality confusion, schema hallucination, and demonstration leakage.

6. Reproducible Pipeline: End-to-end workflow from data preprocessing (SQLite), prompt construction, model inference, to metric computation and result
  visualisation.

