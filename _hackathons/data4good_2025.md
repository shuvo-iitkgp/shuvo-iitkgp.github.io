---
title: "Data4Good 2025 | Building Trust in Educational AI through Factuality Verification"
excerpt: "Built an ensemble factuality-verification pipeline for educational AI responses, achieving **99.03% balanced accuracy** on a held-out competition test set.<br/>Aligned with **UN SDG 4** through safer and more trustworthy AI-assisted learning."
collection: hackathons
---

## Overview

In the **Data4Good Competition (2025)**, our team worked on a socially impactful challenge: reducing misinformation risk in educational AI by verifying whether model-generated answers are factual with respect to supporting context.

Our work, **"Building Trust in Educational AI through Factuality Verification,"** frames the task as a **Natural Language Inference (NLI)** problem and combines transformer-based reasoning with LLM arbitration.

### Team

- **Subhajit Bag**
- **Deepak Alagusubramanian**
- **Aditya Ghosh**
- **Soham Pradhan**

(Georgia Institute of Technology, Atlanta, USA)

---

## Problem & Societal Value

Educational LLM tools are widely used, but fluent yet incorrect responses can reinforce misconceptions and reduce learning quality.

This project targets safer AI deployment by classifying generated answers as:

- **factual**
- **contradiction**
- **irrelevant**

Reliable factuality verification helps platforms decide when to:

- flag outputs for review,
- request additional context,
- or allow direct display to learners.

---

## Dataset

- **21,021** labeled training samples
- **2,000** held-out competition test samples
- Each sample contains: question, context, AI answer, and factuality label
- Strong class imbalance motivated use of **balanced accuracy** as a core metric

---

## Methodology

We developed an **ensemble pipeline**:

- Fine-tuned **DeBERTa-v3-large MNLI** model as the primary factuality classifier
- **GPT-5-mini** arbitration for ambiguous cases
- **SERPAPI-based retrieval augmentation** for low-context instances
- **Human-in-the-loop** review only for rare model disagreement cases

Key insight: retrieval improves performance only when integrated consistently in both training and inference.

---

## Results

- **99.03% balanced accuracy** on the held-out competition test set
- Strong contradiction detection with low disagreement rate between models
- Disagreement cases were rare (~1.3%) and mostly factual-vs-contradiction polarity flips

These results indicate high reliability for gating educational AI responses before they reach learners.

---

## Impact

This work supports **trustworthy AI in education** and aligns with **UN Sustainable Development Goal 4 (Quality Education)**.

At scale, factuality verification can substantially reduce learner exposure to incorrect AI explanations while keeping human review effort small and targeted.

---

## Links

- [Code and Reproducibility](https://github.com/shuvo-iitkgp/Data4Good-2025-Factuality-Detection)
