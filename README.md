# ChildGuard: A Specialized Dataset for Combatting Child-Targeted Hate Speech

ChildGuard is a large, curated, multilingual dataset of 351,877 social media posts, specifically annotated for hate speech targeting children, with detailed age-group labels, sentiment, and contextual features—designed to advance research on online child safety and hate speech detection[1].

---

## 🌟 Key Features

- **Size & Scope:** 351,877 posts from Twitter, Reddit, and YouTube
- **Multilingual:** English and Spanish content
- **Child-Focused:** Explicit labels for three age groups:
  - Teens (13–17)
  - Pre-teens (11–12)
  - Younger children (under 11)
- **Annotations:**
  - Age group, hate/non-hate, explicit/implicit hate
  - Sentiment and polarity scores
  - Platform and context features
- **Data Splits:** Train (70%), Validation (15%), Test (15%)
- **Subsets:** Lexical, Contextual, and Full ChildGuard Dataset

---

## 📂 Dataset Structure

| Column          | Description                                                      |
|-----------------|------------------------------------------------------------------|
| text            | User-generated social media post                                 |
| actual_class    | Ground truth label (Hate/Non-Hate)                               |
| predicted_class | Model-predicted label                                            |
| Age_Group       | Age group of targeted child (Teens, Pre-teens, Younger children) |
| Hate            | 1 for Hate, 0 for Non-Hate                                       |
| ...             | Additional features: sentiment, polarity, platform, etc.         |

---

## 📥 Download

- **Sample:** [Sample 1000 rows](https://gofile.io/d/znYKxX)
- **Full dataset:** Coming soon (upon acceptance).

---

## 🚀 Usage

ChildGuard is intended for academic and research purposes only.  
Potential use cases:
- Benchmarking hate speech detection models
- Studying child-targeted online abuse across age groups
- Developing context-aware moderation tools

---

## 🏆 Baseline Benchmarks

| Model         | Accuracy (Full) | F1 Score (Full) |
|---------------|-----------------|-----------------|
| BERT          | 83.5%           | 82.6%           |
| RoBERTa       | 82.0%           | 81.1%           |
| GPT-3.5-turbo | 80.9%           | 79.9%           |
| LSTM          | 78.3%           | 77.1%           |

*See the paper for detailed results by age group and feature subset.*

---

## 📝 Annotation Guidelines

- Multi-step process: automated preprocessing, manual annotation, consensus review
- Labels: Explicit-Hate, Implicit-Hate, Non-Hate
- High reliability: Cohen’s Kappa = 0.82, Krippendorff’s Alpha = 0.79
- Full guidelines in the [paper][1] (Appendix A.1)

---

## ⚖️ Ethical Statement

All data is anonymized. No personally identifiable information is included.  
Sensitive content is handled with care and in compliance with privacy laws and ethical standards.

---
