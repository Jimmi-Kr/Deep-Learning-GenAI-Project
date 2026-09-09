---
layout: default
title: Milestones
permalink: /milestones.html
---
{% include nav.html %}
{% include eval_banner.html %}

# Milestone Plan

> This term's project is centered on an MCQ-style reasoning task, moving from classic NLP baselines through transformers, RAG, and fine-tuning, to a final ensembled submission. **This page is rewritten each term** since the technical arc of the project changes — unlike the dates/links elsewhere, it isn't pulled from `term.yml`.

| Milestone | Deadline | Focus |
|---|---|---|
| Milestone 0 | Jun 22, 2026 | **Orientation & Setup** — attend orientation, create Kaggle/GitHub/W&B accounts, verify environment access |
| Milestone 1 | Jun 24, 2026 | **NLP Foundation & Semantic Similarity** — text cleaning, tokenization, missing data; TF-IDF/Word2Vec embeddings; cosine similarity between prompt & options; mAP@3 |
| Milestone 2 | Jul 1, 2026 | **Enter the Transformers** — Hugging Face `transformers`/`datasets`; BERT/RoBERTa & attention; context-aware embeddings; zero-shot classification with SLMs |
| Milestone 3 | Jul 8, 2026 | **Context Augmentation with RAG** — limitations of general LLMs; RAG pipeline basics; loading a vector database; retrieving context to improve reasoning |
| Milestone 4 | Jul 15, 2026 | **Formulating the MCQ Task & Fine-Tuning** — data formatting for MCQ; LoRA vs. full fine-tuning; training loop setup; GPU memory & batch size management |
| Milestone 5 | Jul 21, 2026 | **Ensembling** — extracting/sorting logits for top-3 predictions; ensembling strategies across multiple models |
| Last Submission | Jul 26, 2026 | **Final Submission & Presentation** — final Kaggle submission; report with Macro F1 & error analysis; optional deployment via Streamlit/Gradio |

Each milestone builds on the previous one — don't skip ahead without a working checkpoint from the one before.
