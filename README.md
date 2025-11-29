# Hybrid-News-Headline-Generation

---

## 📌 Project Overview

This project performs **automatic text summarization** on a large news dataset.  
It combines traditional word embeddings (**fastText**) with state-of-the-art transformer-based summarization (**Flan-T5**) to generate concise summaries from long news articles.

The project demonstrates a complete NLP pipeline including preprocessing, embedding generation, model loading, and summarization output.

---

## 🎯 Objective

To build an efficient text-summarization system that:

- Understands long news articles  
- Generates high-quality, human-like summaries  
- Combines embedding techniques (fastText) with transformer models (Flan-T5)  
- Demonstrates real-world NLP workflow  

---

## 🧠 Key Features

- fastText word embeddings for text representation  
- Flan-T5 transformer model for abstractive summarization  
- Preprocessing: cleaning, tokenizing, normalization  
- Works on real news dataset with headlines + article text  
- Produces short, meaningful summaries  
- Jupyter Notebook implementation for easy execution  

---

## 🛠 Tech Stack

- **Python**
- **pandas, NumPy**
- **fastText**
- **Transformers (Hugging Face)**
- **Flan-T5**
- **NLTK / regex**
- **Jupyter Notebook**

---

## 📂 Dataset

The dataset used: **`news_summary_more.csv`**  
**It contains**:

- `headlines`: Short article headline  
- `text`: Full news article text  

**Sample**:

`Headline`: Kunal Shah's credit card bill payment platform, CRED, gave users a chance to win free food from Swiggy for one year. Pranav Kaushik, a Delhi techie, bagged this reward after spending 2000 CRED coins. Users get one CRED coin per rupee of bill paid, which can be used to avail rewards from brands like Ixigo, BookMyShow, UberEats, Cult.Fit and more.

`Text`: Delhi techie wins free food from Swiggy for one year on CRED

---

## ⚙️ NLP Pipeline

### 1️⃣ Data Preprocessing
- Lowercasing  
- Punctuation removal  
- Stopword removal  
- Cleaning HTML / URLs  
- Tokenization  

### 2️⃣ fastText Embedding
- Loaded pre-trained **fastText crawl vectors** (2M word vectors)  
- Generated numerical vector representations for each text  
- Used embeddings for semantic understanding  

### 3️⃣ Abstractive Summarization (Flan-T5)
- Loaded model: `google/flan-t5-base`  
- Tokenized article text  
- Generated summaries using T5’s encoder-decoder transformer  
- Post-processed outputs for readability  

### 4️⃣ Evaluation & Output
- Summaries generated for both headlines + article body  
- Compared original text vs generated summaries  
- Exported sample outputs for validation  

---

## 📁 Project Structure

text-summarization/
│── Text_Summarization_using_fastText_and_Flan_t5.ipynb

│── news_summary_more.csv

│── README.md

│── requirements.txt

---

## ▶️ How to Run Locally

### 1. Install dependencies

pip install -r requirements.txt

### 2. Open the notebook

jupyter notebook "Text_Summarization_using_fastText_and_Flan_t5.ipynb"

### 3. Run all cells

This will:
✔ Load fastText embeddings
✔ Load Flan-T5 model
✔ Generate summaries

---

🚀 **Future Enhancements**

Deploy summarizer using Streamlit

Add ROUGE/BLEU evaluation metrics

Use larger models (Flan-T5-large / T5-3B)

Add extractive + abstractive hybrid summarization

Build API endpoint for real-time summarization

---

👤 **Author**

**Srikanth Edigi**

📧 **Email**: srikanthgoud9515@gmail.com

🔗 **LinkedIn**: http://www.linkedin.com/in/srikanth-edigi-4739b125b 
