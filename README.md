# 911 Interactions Analysis


## Leveraging Natural Language Processing and Machine Learning to Accelerate Life-Saving 911 Care


### Problem Statement
The 911 emergency system faces a significant risk of mishaps due to understaffing and the limitations of human dispatchers when handling emergency calls.

### Goals
Develop a real-time machine learning model to support dispatchers in accurately determining the required emergency services for incidents like heart-attacks, strokes, cardiac arrest, and trauma.

Create a scoring system to evaluate the quality of dispatcher decision-making, aiming to enhance emergency response outcomes.

### Project Overview
This project addresses the critical challenge of optimizing emergency response by employing Natural Language Processing and Machine Learning techniques. Here's a brief summary of our progress:

### Achievements
1. Datasets
The project encompasses two vital datasets:
The first comprises audio files.
The second is the EMS dataset.

2. Data Alignment
Our primary objective was to synchronize audio files with their corresponding "First Impression" data available within the EMS dataset through address mapping.

3. Methodologies
We employed several methodologies including FuzzyMatcher, Cosine Similarity Index, and KNN over Cosine Similarity.

4. Comparison
After thorough evaluation, the KNN over Cosine Similarity emerged as the superior approach.

5. Category Consolidation
Initially, there were 120 distinct call categories. We undertook an effort to minimize the total number of categories by grouping similar ones together and eliminating redundant categorizations through text cleaning.

6. NER Model Integration
We incorporated the en_ner_bc5cdr_md model, a named entity recognition (NER) model specialized in the biomedical domain. This model was trained on the BioCreative V Chemical Disease Relation (BC5CDR) corpus, enabling identification of chemical and disease entities and their relationships.

7. Key Features Extraction
The model extracts two essential columns:
Key_words_chemicals
Key_words_disease

8. Model Comparison
After comparing the outputs from various models, we determined that both SVC and NB perform similarly on the dataset. Notably, embeddings outperformed count vectors.

9. Cosine Similarity Enhancement
Implementing Cosine similarity provided significant improvements over fuzzy logic. However, employing KNN over Cosine Similarity yielded substantially superior results.

### Next Steps
Continuous refinement and optimization of models for even more accurate and efficient emergency response.
Exploring additional data sources and techniques to further enhance performance.



