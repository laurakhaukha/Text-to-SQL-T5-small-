## Schema-Augmented Prompt Engineering for Text-to-SQL Generation over SNOMED CT

This repository contains the full code, handcrafted prompts (NL-SQL pairs), and an evaluation pipeline for both few-shot & zero-shot prompting from my MSc Health Data Science dissertation. The project investigates whether schema-augmented prompt engineering (few-shot & zero-shot) can improve SQL generation from natural language (NL) questions for SNOMED CT, using the lightweight T5-small model. Below is an illustration of the user-model (t5-small) interacton for SNOMED-CT via Text-to-SQL.





   <img width="660" height="319" alt="Screenshot 2018-01-18 at 16 57 38" src="https://github.com/user-attachments/assets/f3c5df5d-d3a4-43a0-a6de-6cc21dd4a5fd" />



# Key Components:
1. Schema-Augmented Prompting: Embeds the SNOMED CT schema (description & relationship tables) into prompts to guide SQL generation.
2. Few-Shot vs. Zero-Shot Comparison: Evaluates the impact of K=3 in-context examples per query category on executability and syntactic similarity.
3. Handcrafted NL–SQL Dataset: 120 balanced examples across six clinically motivated categories (e.g., concept lookups, synonym
   retrieval, hierarchical relationship exploration, aggregation queries).
5. Evaluation Framework: Includes Execution Accuracy (EA), Exact Match Accuracy (EMA), Average Sequence Match Score (ASMS), SQLGlot
   semantic equivalence, and Datacompy-based result set comparisons.
6. Error Analysis: Identifies key failure patterns, including directionality confusion, schema hallucination, and demonstration leakage.
7. Reproducible Pipeline: End-to-end workflow from data preprocessing (SQLite), prompt construction, model inference, to metric computation and result
  visualisation.



