# ChildGuard: A Specialized Dataset for Combatting Child-Targeted Hate Speech

![ChildGuard Logo](https://img.shields.io/badge/dataset-childguard-blue)  
*Making the digital world safer for children through data-driven research.*

---

## Overview

**ChildGuard** is a large-scale, multilingual dataset curated to advance research in detecting hate speech specifically targeting children. With 351,877 annotated social media posts, ChildGuard fills a critical gap by providing age-specific, context-rich, and expert-validated resources for developing robust hate speech detection systems.

---

## Key Features

- **Size & Scope:** 351,877 social media posts from Twitter, Reddit, and YouTube
- **Multilingual:** English and Spanish content
- **Child-Focused:** Explicit labeling for three age groups:
  - Teens (13–17)
  - Pre-teens (11–12)
  - Younger children (under 11)
- **Rich Annotations:**
  - Age group, sentiment, polarity, platform, explicit/implicit hate
  - Lexical and contextual features
- **Expert Annotation:** High inter-annotator agreement (Cohen’s Kappa: 0.82, Krippendorff’s Alpha: 0.79)
- **Ethical & Privacy-Compliant:** All personal data anonymized and sensitive content handled per ethical standards

---

## Dataset Structure

| Column         | Description                                                      |
|----------------|------------------------------------------------------------------|
| text           | User-generated social media post                                 |
| actual_class   | Ground truth label (Hate/Non-Hate)                               |
| predicted_class| Model-predicted label                                            |
| Age_Group      | Targeted age group (Teens, Pre-teens, Younger children)          |
| Hate           | Binary indicator: 1 for Hate, 0 for Non-Hate                     |

- **Data splits:** Training (70%), Validation (15%), Testing (15%)
- **Subsets:** Contextual, Lexical, and Full ChildGuard Dataset

---

## Download

- **Sample & Annotation Guidelines:** [Sample Data (GoFile)](https://gofile.io/d/znYKxX)
- **Full Dataset:** To be released upon acceptance (see [ARR_MAY_2025_Dataset.pdf][1])

---

## Usage

ChildGuard is intended for academic, research, and non-commercial use.  
Potential applications include:

- Training and benchmarking hate speech detection models
- Studying age-specific and platform-specific hate speech trends
- Developing safer, context-aware moderation tools

---

## Baseline Benchmarks

| Model          | Accuracy (Full) | F1 Score (Full) |
|----------------|-----------------|-----------------|
| BERT           | 83.5%           | 82.6%           |
| RoBERTa        | 82.0%           | 81.1%           |
| GPT-3.5-turbo  | 80.9%           | 79.9%           |
| LSTM           | 78.3%           | 77.1%           |

*See [ARR_MAY_2025_Dataset.pdf][1] for detailed results by age group and feature subset.*

---

## Annotation Guidelines

- **Explicit-Hate:** Direct abuse or hostile language targeting children
- **Implicit-Hate:** Indirect hostility (sarcasm, coded language, hostile metaphors)
- **Non-Hate:** Neutral, positive, or irrelevant content
- **Quality Control:** Dual annotation, consensus review, and regular audits
- **Ethics:** All PII removed; annotators trained for sensitivity and allowed to opt out of distressing content

---

## Citation

If you use ChildGuard in your research, please cite:


---

## Ethical Statement

ChildGuard was developed in strict compliance with privacy and ethical standards. All data is anonymized, and annotation was performed by trained experts under robust guidelines to ensure the safety and dignity of children represented in the data.

---

## License

Released for research and educational use only.  
For licensing questions, please contact the authors.

---

## Contact

For questions, feedback, or collaboration inquiries, contact the corresponding author:  
**Jiechao Gao** (jiechao@stanford.edu)

---

*ChildGuard: Enabling safer digital spaces for children through research and innovation.*

---

