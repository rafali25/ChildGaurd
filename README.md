# ChildGuard: A Specialized Dataset for Combatting Child-Targeted Hate Speech

---

## Overview

**ChildGuard** is a large, multilingual, and expertly-annotated dataset designed to advance research in detecting hate speech targeting children. With 351,877 curated social media posts, ChildGuard fills a critical gap by providing age-specific annotations, nuanced context, and robust benchmarks for child-focused online abuse detection.

---

## Key Features

- **Size & Scope:** 351,877 user-generated posts from Twitter, Reddit, and YouTube
- **Multilingual:** English and Spanish content
- **Age-Specific Annotations:**  
  - Teens (13–17)  
  - Pre-teens (11–12)  
  - Younger children (under 11)
- **Rich Metadata:**  
  - Age group, sentiment, polarity, platform, explicit/implicit hate
- **Expert Annotation:**  
  - High inter-annotator agreement (Cohen’s Kappa: 0.82, Krippendorff’s Alpha: 0.79)
- **Ethical & Privacy-Compliant:**  
  - All personal data anonymized and sensitive content handled per ethical standards

---

## Dataset Structure

| Column           | Description                                               |
|------------------|----------------------------------------------------------|
| text             | Social media post                                        |
| actual_class     | Ground truth label (Hate/Non-Hate)                       |
| predicted_class  | Model-predicted label                                    |
| Age_Group        | Age group of targeted child (Teens, Pre-teens, Younger)  |
| Hate             | Binary indicator: 1 (Hate), 0 (Non-Hate)                 |
| ...              | Additional features: sentiment, polarity, platform, etc. |

- **Data splits:** Training (70%), Validation (15%), Testing (15%)
- **Subsets:** Contextual, Lexical, and Full ChildGuard Dataset

---

## Download

- **Full dataset and documentation:** To be released upon acceptance.
- **Sample & annotation guidelines:** [Sample link](https://gofile.io/d/znYKxX)
- **Paper:** See `ARR_MAY_2025_Dataset.pdf` for full methodology and statistics.

---

## Usage

ChildGuard is intended for academic, research, and non-commercial use.  
Example use cases:
- Training and benchmarking hate speech detection models
- Studying the impact of online hate on children
- Developing context-aware, platform-specific moderation tools

---

## Baseline Benchmarks

| Model         | Accuracy (Full) | F1 Score (Full) |
|---------------|-----------------|-----------------|
| BERT          | 83.5%           | 82.6%           |
| RoBERTa       | 82.0%           | 81.1%           |
| GPT-3.5-turbo | 80.9%           | 79.9%           |
| LSTM          | 78.3%           | 77.1%           |

*See the paper for detailed results across age groups and feature subsets.*

---

## Citation

If you use ChildGuard in your research, please cite:

@inproceedings{childguard2025,
  title={ChildGuard: A Specialized Dataset for Combatting Child-Targeted Hate Speech},
  author={Gautam Siddharth Kashyap and Mohammad Anas Azeez and Rafiq Ali and Zohaib Hasan Siddiqui and Jiechao Gao and Usman Naseem},
  year={2025},
  note={arXiv preprint}
}




---

## Ethical Statement

ChildGuard was developed in strict accordance with privacy and ethical standards. All personal identifiers were removed, and annotation was performed by trained experts under robust guidelines to ensure the safety and dignity of children represented in the data.

---

## License

This dataset is released for research and educational use only.  
For licensing questions, please contact the authors.

---

## Contact

For questions, feedback, or collaboration inquiries, please contact the author:  
**Rafiq Ali** (rafworkacc@gmail.com)

---

*ChildGuard: Enabling safer digital spaces for children through research and innovation.*

---
