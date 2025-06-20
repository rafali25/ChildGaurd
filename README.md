# 🛡️ ChildGuard: A Specialized Dataset for Combatting Child-Targeted Hate Speech

![ChildGuard Banner](https://imgur.com/placeholder-banner.png)

---

## 📚 Overview

**ChildGuard** is a large-scale, multilingual dataset meticulously curated to advance research on hate speech detection specifically targeting children. With over **350,000** annotated social media posts, ChildGuard fills the critical gap in age-specific, context-rich, and ethically sourced data for online safety research.

---

## ✨ Key Features

- **Size & Scope:** 351,877 posts from Twitter, Reddit, and YouTube
- **Multilingual:** English & Spanish
- **Child-Focused:** Explicitly targets hate speech directed at children, segmented by age:
  - Teens (13–17)
  - Pre-teens (11–12)
  - Younger children (under 11)
- **Rich Annotations:**
  - Age group labels
  - Lexical and contextual features
  - Sentiment & polarity scores
  - Explicit vs. implicit hate
- **Expert-Validated:** High inter-annotator agreement (Cohen’s Kappa = 0.82, Krippendorff’s Alpha = 0.79)
- **Ethical & Privacy-Compliant:** All personal data anonymized and sensitive content handled per ethical guidelines

---

## 🗂️ Dataset Structure

| Column           | Description                                             |
|------------------|--------------------------------------------------------|
| text             | User-generated social media post                       |
| actual_class     | Ground truth label (Hate/Non-Hate)                     |
| predicted_class  | Model-predicted label                                  |
| Age_Group        | Age group (Teens, Pre-teens, Younger children)         |
| Hate             | Binary indicator: 1 for Hate, 0 for Non-Hate           |
| ...              | Additional features: sentiment, polarity, platform, etc.|

- **Data splits:** Training (70%), Validation (15%), Testing (15%)
- **Subsets:** Contextual, Lexical, and Full ChildGuard Dataset

---

## 🚀 Download

- **Sample data & annotation guidelines:** [Sample Download](https://gofile.io/d/znYKxX)
- **Full dataset:** To be released upon acceptance

---

## 🛠️ Usage

ChildGuard is intended for academic, research, and non-commercial purposes.

**Use Cases:**
- Training & benchmarking hate speech detection models
- Studying the impact of online hate on children by age group
- Developing context-aware, platform-specific moderation tools

---

## 📊 Baseline Benchmarks

| Model          | Accuracy | F1 Score |
|----------------|----------|----------|
| BERT           | 83.5%    | 82.6%    |
| RoBERTa        | 82.0%    | 81.1%    |
| GPT-3.5-turbo  | 80.9%    | 79.9%    |
| LSTM           | 78.3%    | 77.1%    |

*See the paper for detailed results across age groups and feature subsets.*

---

## 📝 Citation

If you use ChildGuard in your research, please cite:

