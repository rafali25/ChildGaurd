# ChildGuard Dataset

A specialized dataset for detecting and analyzing child-targeted hate speech online.

## Table of Contents

1. [Overview](#overview)
2. [Dataset Structure](#dataset-structure)
   * [Lexical Subset](#lexical-subset)
   * [Contextual Subset](#contextual-subset)
   * [Full ChildGuard Dataset](#full-childguard-dataset)
3. [Key Statistics](#key-statistics)
4. [Data Fields](#data-fields)
5. [Usage](#usage)
6. [Citation](#citation)
7. [Contact](#contact)

## Overview

The **ChildGuard** dataset is a curated collection of social media and online content specifically annotated to detect hate speech aimed at minors. Built upon a range of existing corpora, ChildGuard enriches samples with age-based labels, sentiment scores, and contextual features to empower researchers and developers focused on protecting children in digital environments.

**Authors**: Gautam Siddharth Kashyap, Mohammad Anas Azeez, Rafiq Ali, Zohaib Hasan Siddiqui, Jiechao Gao, Usman Naseem.

**Paper:** [arXiv preprint (PDF)](https://arxiv.org/pdf/2506.21613) | [arXiv abstract (latest)](https://arxiv.org/abs/2506.21613v1)

## Dataset Structure

ChildGuard is divided into three main subsets to support different analytical approaches:

### Lexical Subset

- **Rows:** 157,280
- **Columns:** `text`, `actual_class`, `predicted_class`, `Hate` (1 = hate, 0 = non-hate)
- **Description:** Focuses on word-level features (vocabulary richness, sentiment). No age labels.

### Contextual Subset

- **Rows:** 194,597
- **Columns:** `text`, `actual_class`, `predicted_class`, `Age_Group`, `Hate` (1 = hate, 0 = non-hate)
- **Description:** Adds age-based categories and platform-specific context scores for deeper semantic analysis.

### Full ChildGuard Dataset

- **Rows:** 351,877
- **Columns:** `text`, `actual_class`, `predicted_class`, `Age_Group`, `Hate` (1 = hate, 0 = non-hate)
- **Description:** Integrates both lexical and contextual annotations, covering three age groups:
  - Teens (13–17)
  - Pre-teens (11–12)
  - Younger Children (< 11)

## Key Statistics

| Metric                      | Lexical | Contextual | ChildGuard |
|-----------------------------|:-------:|:----------:|:----------:|
| Unique Words                | 28,764  | 22,890     | 35,412     |
| Average Text Length (words) | 19.1    | 22.7       | 21.2       |
| Proportion Explicit Hate    | 26%     | 24%        | 25%        |
| Proportion Implicit Hate    | 12%     | 14%        | 13%        |

## Data Fields

- **text**: The raw user-generated statement.
- **actual_class**: Ground truth label (Hate vs. Non-Hate).
- **predicted_class**: Model-predicted label for comparative evaluation.
- **Hate**: Binary indicator (1 = Hate; 0 = Non-Hate).
- **Age_Group**: Age category for contextual analysis (Teens, Pre-Teens, Younger Children).

## Usage

This repository includes three key CSV files, each serving a specific subset of the ChildGuard data:

1. **`contextual_childhate.csv`**
   - **Rows:** 194,597
   - **Columns:**
     - `text`: Raw user-generated statements.
     - `actual_class`: Ground truth label (`Hate` vs. `Non-Hate`).
     - `predicted_class`: Model-predicted label.
     - `Age_Group`: Annotated age category (Teens, Pre-Teens, Younger Children).
     - `Hate`: Binary indicator (1 = Hate; 0 = Non-Hate).
   - **Description:** Contains context-enriched samples with age labels for semantic analysis.

2. **`lexical_childhate.csv`**
   - **Rows:** 157,280
   - **Columns:**
     - `text`: Raw user-generated statements.
     - `actual_class`: Ground truth label (`Hate` vs. `Non-Hate`).
     - `predicted_class`: Model-predicted label.
     - `Hate`: Binary indicator (1 = Hate; 0 = Non-Hate).
   - **Description:** Focuses on word-level (lexical) features without age annotations.

3. **`childguard_dataset.csv`**
   - **Rows:** 351,877
   - **Columns:**
     - `text`: Raw user-generated statements.
     - `actual_class`: Ground truth label (`Hate` vs. `Non-Hate`).
     - `predicted_class`: Model-predicted label.
     - `Age_Group`: Annotated age category (Teens, Pre-Teens, Younger Children).
     - `Hate`: Binary indicator (1 = Hate; 0 = Non-Hate).
   - **Description:** The full combined dataset integrating both lexical and contextual annotations.

## Citation

If you use the ChildGuard dataset in your research, please cite our paper:
```
@article{childguard2025,
  title={ChildGuard: A Specialized Dataset for Detecting and Analyzing Child-Targeted Hate Speech Online},
  author={Gautam Siddharth Kashyap and Mohammad Anas Azeez and Rafiq Ali and Zohaib Hasan Siddiqui and Jiechao Gao and Usman Naseem},
  journal={arXiv preprint arXiv:2506.21613},
  year={2025},
  url={https://arxiv.org/abs/2506.21613v1}
}
```




## Contact

For questions or collaboration inquiries, please contact:

- **Rafiq Ali** – [rafworkacc@gmail.com](mailto:rafworkacc@gmail.com)

*Last updated: June 2025*
