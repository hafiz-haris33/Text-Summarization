# 📝 Text Summarization using CNN/DailyMail Dataset

This project is part of an internship task to build a text summarization system that converts lengthy news articles, blogs, or reports into concise summaries using both extractive and abstractive approaches.

## 📌 Objective

To develop a robust summarization pipeline using:
- **Extractive Summarization** (with spaCy)
- **Abstractive Summarization** (using Transformers like BART)
- **Fine-tuning** on the CNN/Daily Mail dataset
- **Evaluation** with ROUGE metrics

---

## 📂 Folder Structure

text-summarization-project/
* requirements.txt # Python dependencies
* README.md # Project documentation
* Project Report.docx
* notebook.ipynb


---

## 📚 Dataset

- **Name**: CNN/DailyMail Dataset
- **Source**: HuggingFace Datasets
- **Description**: A large collection of news articles and corresponding highlights used for summarization tasks.

---

## 🚀 Project Steps

### 1. Preprocessing
- Loading CNN/DailyMail via HuggingFace
- Cleaning and preparing text (tokenization, truncation)

### 2. Extractive Summarization (spaCy)
- Named Entity Recognition & sentence extraction using spaCy
- Rule-based summarizer that selects key sentences

### 3. Abstractive Summarization (Transformers)
- Used pre-trained `facebook/bart-base` model
- Generated summaries using `transformers.pipeline`

### 4. Fine-Tuning
- Fine-tuned BART model on a subset of CNN/DailyMail
- Trained for 1 epoch to improve relevance of summaries

### 5. Real-World Testing + Evaluation
- Inputted real-world news articles
- Evaluated generated summaries using ROUGE metrics:

rouge1: 0.2832
rouge2: 0.1016
rougeL: 0.1919
rougeLsum: 0.2348


---

## 📈 Evaluation Metric

We used the **ROUGE** (Recall-Oriented Understudy for Gisting Evaluation) metric:
- `rouge1` – Overlap of unigrams
- `rouge2` – Overlap of bigrams
- `rougeL` – Longest common subsequence
- `rougeLsum` – Variant suitable for summarization tasks

---

## 🧪 Sample Results

| 🔹 Article | 🟢 Generated Summary |
|-----------|----------------------|
| Federal judge halted ban on Harvard | Judge blocked Trump’s policy against international students, calling it retaliation. |
| Russia-Ukraine prisoner swap | Over 1500 prisoners released as part of the ongoing exchange between nations. |

---

## 🛠️ Tech Stack

- Python
- Jupyter Notebooks
- HuggingFace Transformers & Datasets
- spaCy
- PyTorch
- ROUGE metric (`evaluate` library)

---

## 📌 Installation

```bash
# Clone the repository
git clone https://github.com/Hafi-haris33/Text-Summarization.git
cd Text-Summarization

# Install dependencies
pip install -r requirements.txt
```
---


🙌 Acknowledgements
HuggingFace Datasets
Transformers by HuggingFace
spaCy NLP

👨‍💻 Author
Name: Hafiz Muhammad Haris Attique
🔗 [LinkedIn](https://www.linkedin.com/in/hafiz-muhammad-haris-305211361)
