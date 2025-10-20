# linked-insights-ner: Extracting Job Skills from LinkedIn Postings with spaCy

> **A custom Named Entity Recognition (NER) model built with spaCy to automatically extract professional skills from job postings.**

---

## Overview

This is a natural language processing project that uses **spaCy** to detect and extract technical and analytical skills from job descriptions.  

By training a custom NER model, the project converts unstructured text into structured skill data that can power downstream analytics — such as skill co-occurrence networks, salary modeling, and career path recommendations.

---

## Project Goals

- Fine-tune a **spaCy NER model** to recognize skill entities (e.g., “Python”, “TensorFlow”, “Power BI”).  
- Create a **reusable pipeline** for text cleaning, annotation, and model evaluation.  
- Demonstrate entity extraction on real LinkedIn-style job postings.  
- Provide foundations for downstream analyses like skill networks or salary insights.

---

## 🧩 Project Structure
```
├── data/
│
├── notebooks/
│ ├── 01_exploring_linkedin_data.ipynb
│ ├── 02_generate_NER_and_label_data.ipynb
│ └── 03_generate_similarity_recommendations.ipynb
│
├── models/
│ └── ner_skill_model/ # Saved spaCy pipeline
│
└── README.md
---

```

---

## ⚙️ Tech Stack

| Category | Tools / Libraries |
|-----------|-------------------|
| **Language Processing** | spaCy (NER, tokenization, model training) |
| **Data Handling** | pandas, json, regex |
| **Evaluation** | spaCy Scorer (precision, recall, F1) |
| **Visualization** | spaCy displaCy, matplotlib, seaborn |

---

## Lessons Learned

* Clean annotation boundaries are critical for NER accuracy — even minor character misalignments can fail training
* Custom skill extraction works best when domain-specific terms are represented in training data
* Transfer learning (starting from en_core_web_md or en_core_web_lg) improves recall for real-world phrasing
* Skill tagging generalizes well to unseen postings after ~500–1000 quality annotations.

## Summary

This project demonstrates:
* Custom NER training with spaCy
* Handling and validating annotated data
* Model evaluation and interpretability
* Turning unstructured text into structured, analyzable skill data
* Data validation, preparation, and cleaning

## Author

Jennifer Podracky
Data Scientist | Product & Program Analytics
