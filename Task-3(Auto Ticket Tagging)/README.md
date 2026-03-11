# Auto Tagging Support Tickets Using LLM

## Project Overview

Customer support systems receive a large number of user queries every day. Manually reading and categorizing these support tickets into appropriate categories is time-consuming and inefficient.

This project builds an **automated support ticket tagging system using a Large Language Model (LLM)**. The system analyzes the text of a support ticket and predicts the **top three most relevant categories** for that ticket.

The goal is to demonstrate how **Large Language Models can automate ticket categorization and improve customer support workflows.**

---

## Objective

The main objective of this project is to **automatically classify customer support tickets into relevant categories using an LLM**.

The system reads the ticket text and predicts the **top three most probable tags**. The project also compares **Zero-Shot Learning** and **Few-Shot Learning** approaches to analyze how providing example tickets affects model predictions.

---

## Dataset Used

This project uses the **Banking77 dataset**, which contains real customer service queries related to banking applications.

Examples of issues in the dataset include:

* Account access problems
* Card-related issues
* Payment and billing problems
* Transaction errors
* Security and fraud concerns

In this project, each query is treated as a **support ticket** that needs to be automatically categorized.

---

## Model Used

The project uses a **pre-trained transformer model for zero-shot text classification**.

**Model:**
`distilbert-base-uncased-mnli`

This model is trained on the **MultiNLI (Natural Language Inference) dataset** and can classify text into categories without being specifically trained on the target dataset.

---

## Tools and Technologies Used

* **Python** – Programming language used for implementation
* **Pandas** – Data manipulation and preprocessing
* **NumPy** – Numerical operations
* **Hugging Face Transformers** – Loading and using pre-trained LLM models
* **PyTorch** – Deep learning framework used by transformer models
* **Jupyter Notebook** – Development environment for experimentation and analysis

---

## Methodology

### 1. Zero-Shot Classification

The model predicts categories for a ticket **without being trained on the dataset**. It compares the ticket text with predefined category labels and ranks them based on relevance.

### 2. Few-Shot Learning

In the few-shot approach, the model is provided with **a few example tickets and their correct tags** before classifying a new ticket. These examples help the model understand the classification task better.

### 3. Top-3 Tag Prediction

For each support ticket, the model returns the **three most relevant predicted categories** instead of just one label.

---

## Example Output

Below is an example of how the system predicts categories for a support ticket.

**Support Ticket:**

```
Is it possible for me to change my PIN number?
```

**Zero-Shot Predicted Tags:**

1. Card Problem
2. Account Access Problem
3. General Inquiry

**Few-Shot Predicted Tags:**

1. Card Problem
2. Account Access Problem
3. Transaction Issue

The model predicts the **top three most relevant categories** for each support ticket. These predictions help support systems automatically route tickets to the correct department.

---

## Results and Observations

Both approaches were evaluated on a subset of support tickets.

* **Zero-Shot Classification** successfully identified general ticket categories.
* **Few-Shot Learning** improved contextual understanding in several cases by providing examples.

Overall, **Few-Shot Learning produced slightly more context-aware predictions compared to Zero-Shot Classification.**

---

## Conclusion

This project demonstrates how **Large Language Models can automate support ticket categorization**. Such systems can significantly improve customer support operations by:

* Automatically routing tickets to the correct department
* Reducing manual tagging effort
* Improving response time for customer issues

---

## Author

**Ume Habiba**
BS Information Technology Student

⭐ If you found this project useful, feel free to star the repository.

