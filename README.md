# NLP Text Vectorization Lab

![NLP](https://img.shields.io/badge/Focus-Natural%20Language%20Processing-green)
![Python](https://img.shields.io/badge/Language-Python%203.12-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)

This repository contains a comprehensive exploration of **Natural Language Processing (NLP)** foundations, focusing on text preprocessing and feature extraction. The project demonstrates how to transform raw, unstructured text into structured numerical formats suitable for machine learning models.

---

## 🚀 Project Overview
The core objective of this lab was to process a dataset of **labelled sentences** (focused on global health and COVID-19) and apply various vectorization techniques to understand word importance and frequency.

### Key Features:
* **Advanced Text Preprocessing**: Implementation of a cleaning pipeline including lowercasing, regex-based noise removal, tokenization, and stopword filtering.
* **Feature Engineering**: Comparative analysis between **Bag-of-Words (CountVectorizer)** and **TF-IDF (Term Frequency-Inverse Document Frequency)**.
* **Vocabulary Analysis**: Examination of case-sensitive vs. case-insensitive tokenization and its impact on vocabulary size.

---

## 🛠️ Tech Stack
* **Language**: Python
* **Libraries**: 
    * `Pandas` & `Openpyxl`: Data manipulation and Excel handling.
    * `NLTK`: Natural Language Toolkit for tokenization and stopword removal.
    * `Scikit-learn`: Feature extraction and vectorization.
    * `Re`: Regular expressions for advanced text cleaning.

---

## 📊 Dataset Analysis
The analysis was performed on a dataset containing health-related reports.

* **Total Unique Words (Vocabulary)**: ~3,288
* **Top Themes**: The data is heavily centered on the COVID-19 pandemic.
* **Frequent Words**: `covid`, `health`, `cases`, `new`, `vaccine`, and `pandemic`

---

## 📝 Methodology

### 1. Data Loading & Cleaning
Raw sentences were imported from Excel. The preprocessing function handles noise reduction by:
* Converting all text to lowercase.
* Removing non-alphabetic characters (numbers/punctuation).
* Filtering out common English stopwords (e.g., "the", "is", "in").

### 2. Vectorization Techniques
We compared two primary methods for converting text to numbers:

| Method | Description | Use Case |
| :--- | :--- | :--- |
| **CountVectorizer** | Counts raw frequency of each word in a document. | Simple frequency analysis. |
| **TF-IDF** | Weighs words based on frequency in a document vs. the whole corpus. | Identifying unique/important keywords. |

### 3. Validation
The output was validated by previewing the TF-IDF weight matrices and inspecting the vocabulary mapping to ensure data integrity during the transformation process.

---
