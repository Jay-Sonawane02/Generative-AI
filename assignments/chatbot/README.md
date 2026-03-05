# AI Learning Path Generator

This notebook implements a simple **AI learning assistant** that helps users understand complex topics.

Given a topic as input, the system uses a **Large Language Model (LLM)** to:

1. Identify the **top 5 prerequisite concepts** required to understand the topic.
2. Generate a **short beginner-friendly article** for each concept.

This creates a **structured mini learning path** for the given topic.

---

## Example

**Input**

```
Transformers
```

**Generated Topics**

1. Attention Mechanism
2. Self-Attention
3. Positional Encoding
4. Encoder–Decoder Architecture
5. Tokenization

The notebook then generates explanations for each topic.

---

## Technologies Used

* Python
* Google Gemini API
* Jupyter Notebook

---

## How to Run

Install dependency:

```
pip install google-generativeai
```

Open the notebook:

```
chatbot.ipynb
```

Run the cells and enter a topic when prompted.

---

