# Interview Question Tagger using Zero-Shot Classification

This project automatically **classifies interview questions into relevant topics** using a combination of **LLM-based category discovery** and **zero-shot classification**.

The dataset contains interview questions instead of manually defining categories, an LLM is first used to **discover the main topics present in the dataset**, and a zero-shot classification model is then used to tag each question.

---

## Workflow

```
CSV Dataset
      ↓
Random sample (100 questions)
      ↓
LLM extracts topic categories
      ↓
Zero-shot classification model
      ↓
Each question assigned a category
```

---

## Libraries Required

Install the required libraries before running the notebook:

```bash
pip install pandas transformers torch tqdm google-genai
```

Main libraries used:

* **pandas** – dataset handling
* **transformers** – Hugging Face zero-shot classification pipeline
* **torch** – deep learning backend
* **tqdm** – progress tracking
* **google-genai** – LLM API for category discovery

---

## How to Run

1. Install the required dependencies.
2. Open the notebook in **Jupyter Notebook or VS Code**.
3. Place the dataset (`data_science.csv`) in the project directory.
4. Run the cells sequentially to:

   * Discover categories using the LLM
   * Perform zero-shot classification
   * Generate tagged interview questions.

---


