# LLM-Bodywash Review Classification (Groq + LLaMA)

## Project Goal
This project performs **multi-label classification** of product reviews (bodywash reviews) into **Level 1 (PARENT) ** and **Level 2 (CHILD)** category labels using **LLMs (Groq + LLaMA)**.

---

## Problem Statement
Given a dataset of bodywash product reviews, predict the correct Level 1 and Level 2 category using any LLM model which is suited for NLP task without using BERT.
---

## 🛠️ Tech Stack

- **LLM Model**: Groq + LLaMA (LLaMA-3 on Groq API)
- **Language**: Python (Jupyter Notebook)
- **Libraries**: `pandas`,`sklearn`, `Groq API`, `json`
- **Data**: Product review dataset with labeled training and unlabeled test samples
- **Methods**:
  - Few-shot prompting
  - Semantic similarity (optional with FAISS)
  - Evaluation: Precision, Recall, F1-score, Jaccard
---

## 📂 Files

| File                          | Description                                       |
|-------------------------------|---------------------------------------------------|
| `LLMProject.ipynb`            | Jupyter notebook for data processing and prediction using LLM |
| `bodywash-train.xlsx`         | Training data with ground truth Level 1 & Level 2 |
| `bodywash-test.xlsx`          | Test data with reviews only                      |
| `bodywash_predictions_filled.xlsx` | Final predictions with both labels         |
| `README.md`                   | Project documentation                             |

---

## 🚀 Approach

1. **Prompt Engineering**: Designed context-rich prompts for few-shot learning.
2. **LLM Inference**: Called Groq API with LLaMA for label generation.
3. **Postprocessing**: Parsed and validated LLM outputs.
4. **Output Generation**: Saved predictions in Excel format.

---

## 📈 Results

- The model generated consistent and relevant category labels for unseen reviews.
- Demonstrated the viability of using LLMs for multi-label classification tasks with minimal training.
- Level 1 Accuracy: 85%
- Level 2 Accuracy: 79%
---

## ✅ To Do

- [ ] Evaluate performance quantitatively (accuracy, F1)
- [ ] Add more robust error handling
- [ ] Include prompt templates in separate script

---

## 🧠 Author

Shreya Chaudhary
LinkedIn: 
 

