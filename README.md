# Scientific Literature Mining 

A research-driven project aimed at mining scientific literature using unsupervised learning techniques, incorporating knowledge graphs for deeper contextual understanding, and leveraging prompting strategies (zero-shot/few-shot) with LLMs. Our goal is to uncover research trends, enhance literature comprehension, and diagnose LLM failures through targeted domain experiments.

---

## Project Overview

This project explores the intersection of **Unsupervised Learning**, **Large Language Models (LLMs)**, and **Knowledge Graphs** to:

- Identify emerging **research trends** from large-scale academic literature (e.g., arXiv).
- Extract and build **domain-specific knowledge graphs** for improved context and semantic clarity.
- Experiment with **prompting strategies** (zero-shot, few-shot) to evaluate literature comprehension capabilities of LLMs.
- Conduct **domain-specific evaluations** to analyze and interpret LLM failures when answering scientific questions.
- Automate **ArXiv literature extraction** and metadata parsing for NLP-ready pipelines.

---

## Key Components

### 1. Unsupervised Learning for Trend Mining
- Topic modeling (e.g., LDA, BERTopic)
- Clustering techniques (e.g., K-Means, HDBSCAN) on document embeddings
- Temporal trend analysis of emerging research themes

### 2. Knowledge Graph Inclusion
- Entity and relation extraction from scientific texts
- Construction of contextualized knowledge graphs (e.g., using Neo4j)
- Graph augmentation using domain-specific ontologies

### 3. Prompt Engineering & Evaluation
- Zero-shot and few-shot prompting using models like GPT-4 and LLaMA
- Comparative analysis of answers across domains
- Case studies highlighting LLM strengths and weaknesses in literature review

### 4. Domain Experiments
- Evaluation metrics for correctness, hallucination, and coverage
- Use of expert feedback to evaluate LLM output

### 5. ArXiv Literature Extraction
- Automated scraping and parsing of ArXiv abstracts and metadata
- PDF-to-text processing 

---

## Tech Stack


---

## Experiments

| Experiment | Domain          | Goal                                | Outcome                              |
|-----------|------------------|-------------------------------------|--------------------------------------|
| Exp1      | NLP              | Test LLM zero-shot on summarization | Moderate performance, factual errors |
| Exp2      | Quantum Physics  | Few-shot prompting for classification | Improved accuracy                  |
| Exp3      | Bioinformatics   | Knowledge graph-enhanced QA         | Contextual responses, some limitations |

---

## Folder Structure

---

## How to Run

1. **Clone the repo**
```bash
git clone https://github.com/dreamboat26/Scientific-Literature-Mining.git
cd -
```

---

## Contributors

- Unsupervised Learning Method for Research Trends - Snehal Rakshit, Varun Ramanathan Alagappan, Vedant Vijay Patil. [Names]
- Knowledge Graphs & Evaluation - [Name] 
- Prompting Techniques for context - Rahul Jaisy, Eishaan Khatri, [Names]
- Arxiv Literature Papers Extraction & QA system - Shinjini Mondal, Archishman Banerjee. [Names]
- Domain Experimentation Team - [Names] , Theo Fraser, Gayathri Aishwarya E, 

---

## Future Work

- Integrate citation graph analysis for trend propagation

---

## License

This project is licensed under the [MIT License](LICENSE).

---
