# Domain Experiments in Scientific Literature Understanding

This module investigates how well Large Language Models (LLMs) and rule-based systems understand domain-specific scientific literature. It includes experiments using **custom prompts**, **automated metrics**, and **rule-based logic** to evaluate the **factual accuracy**, **depth**, and **coherence** of responses.

---

## Objective

To systematically evaluate LLMs across research domains by:

- Designing **question-answering experiments** based on real scientific papers.
- Testing **zero-shot**, **few-shot**, and **chain-of-thought prompting** strategies.
- Incorporating **rule-based baselines** for comparison.
- Using **custom scoring metrics** beyond generic LLM benchmarks.

---

## Focus Areas Targeted

- Do LLMs extract accurate information from scientific papers?
- Where do they hallucinate or misinterpret key concepts?
- Can rule-based systems provide better reliability in specific domains?
- How do different prompting formats affect comprehension?

---

## Domains Covered

- **Quantum Physics**
- **Bioinformatics**

---

## Methods & Techniques Used To Run Experiments

### Prompting Strategies
- **Zero-shot**, **Few-shot**, and **Chain-of-thought**
- Dynamic prompt templates for different task types
- Prompt testing with both general and domain-specific LLMs

### Rule-Based Systems
- Handcrafted rules for extracting answers from abstracts
- Keyword-based logical filters and sentence scoring
- Used as a baseline or fallback model

### Evaluation Metrics Designed
| Metric            | Description                                                  |
|------------------|--------------------------------------------------------------|
| `Relevance Score`| Cosine similarity with reference answer using sentence embeddings |
| `Factual Accuracy`| Binary/manual check for scientific correctness              |
| `Hallucination Rate` | Proportion of generated content not found in source text |
| `Length Ratio`   | Length of answer compared to reference (brevity vs verbosity) |
| `Coherence`      | Logical flow and completeness (manual or LLM-graded)          |

---

## Folder Structure

---

## Sample QA Entry

```json
{
  "domain": "Quantum Physics",
  "question": "What is the main contribution of the paper?",
  "reference_answer": "It proposes a new simulation method for 2D quantum lattice systems...",
  "model_response": "The authors introduce a simulation framework for 2D quantum systems...",
  "relevance_score": 0.89,
  "factual_accuracy": 1,
  "hallucination": 0,
  "length_ratio": 1.1
}
```

---

## Results

| Domain         | Model     | Prompt Type | Accuracy | Hallucination | Rule-Based Score |
|----------------|-----------|-------------|----------|----------------|------------------|
| NLP            | GPT-4     | Few-shot    | X     | X          | X            |
| Bioinformatics | LLaMA-2   | Zero-shot   | X     | X          | X            |
| Quantum Physics| Rule-Based| N/A         | X     | X          | -                |

---

## Features

- Easily extendable to new domains or metrics
- Benchmark comparison with rule-based systems
- Comparing various methods for better analysis

---

## Future Work

- Add scoring models (e.g., GPT-as-a-judge)
- Integrate retrieval-augmented QA (RAG) for grounding

---

## License

MIT License
