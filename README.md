# AI-Powered Paraphrasing Tool

A transformer-based NLP tool that rewrites text while preserving meaning, improving clarity, and ensuring originality — built with Hugging Face Transformers, LanguageTool, and Sentence-Transformers.

**Author:** Muhsina Safeeth


---

## Overview

This project is a Generative AI module assignment that implements an end-to-end paraphrasing pipeline. It uses the **T5-small** transformer model to generate paraphrases, applies automated grammar and fluency correction, and quantitatively evaluates output quality using BLEU, ROUGE-L, and semantic similarity metrics.

## Features

- 🔄 **Transformer-based paraphrasing** using T5-small (task-prefix prompting, no fine-tuning required)
- ✅ **Grammar & spelling correction** via LanguageTool
- 📊 **Quantitative evaluation** with BLEU, ROUGE-L, and semantic similarity scores
- ⚡ **Lightweight & CPU-friendly** — no GPU required
- 📓 **Clean, well-commented notebook** demonstrating the full workflow

## Tech Stack

| Component | Technology |
|---|---|
| Language | Python |
| Paraphrasing Model | T5-small (Hugging Face Transformers) |
| Grammar Checking | LanguageTool |
| Semantic Evaluation | Sentence-Transformers |
| Metrics | BLEU, ROUGE-L, Semantic Similarity |

## Architecture

```
User Input
    │
    ▼
Preprocessing Layer (cleaning, formatting)
    │
    ▼
Transformer Model — T5-small (generates paraphrase)
    │
    ▼
Grammar & Fluency Check — LanguageTool
    │
    ▼
Evaluation Metrics — BLEU | ROUGE | Semantic Similarity
    │
    ▼
Final Output
```

## Why T5-small?

- Efficient and fast in CPU-only environments
- Produces fluent, natural paraphrases
- Beginner-friendly with a simple task-prefix interface
- Works out of the box — no fine-tuning required

## Evaluation Metrics

| Metric | Purpose |
|---|---|
| **BLEU** | Measures word-level similarity between original and paraphrase |
| **ROUGE-L** | Measures longest common subsequence overlap |
| **Semantic Similarity** | Measures meaning preservation using sentence embeddings |

> **Note:** Semantic similarity is the most important metric, since the core goal of paraphrasing is to preserve meaning even as wording changes.

## Example

**Input:**
> Artificial intelligence is transforming many industries by automating tasks, improving decision-making, and enabling new products and services. However, it also raises important ethical and social questions that must be addressed.

**Output (after grammar correction):**
> AI is reshaping several industries by automating work, enhancing decisions, and creating new services and products. At the same time, it brings ethical and social concerns that need careful attention.

**Scores:**

| Metric | Score | Interpretation |
|---|---|---|
| BLEU | 0.42 | Moderate lexical overlap — wording is original |
| ROUGE-L | 0.58 | Key ideas preserved |
| Semantic Similarity | 0.87 | Strong meaning preservation |

### Observations

- The paraphrased text is clearer, more concise, and grammatically correct.
- Grammar correction improved fluency and readability.
- High semantic similarity confirms the meaning remains intact.
- Moderate BLEU and ROUGE scores indicate genuine originality in wording, not just copying.

## Project Outcomes

- ✅ Meaning-preserving paraphrasing
- ✅ Automated grammar correction
- ✅ Quantitative semantic evaluation
- ✅ Full transformer-based NLP workflow
- ✅ Ready for future deployment and enhancement

## Roadmap / Future Enhancements

- [ ] Generate multiple paraphrase variations per input
- [ ] Fine-tune the model on custom/domain-specific datasets
- [ ] Integrate plagiarism detection
- [ ] Deploy as a web API or CLI application
- [ ] Add multilingual paraphrasing support

## References

1. Raffel, C., et al. (2020). *Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer (T5)*.
2. Hugging Face Transformers Documentation.
3. LanguageTool Documentation.
4. Sentence-Transformers Documentation.
5. Papineni, K., et al. (2002). *BLEU: A Method for Automatic Evaluation of Machine Translation*.
6. Lin, C.-Y. (2004). *ROUGE: A Package for Automatic Evaluation of Summaries*.

---

*Module End Assignment — Generative AI*
