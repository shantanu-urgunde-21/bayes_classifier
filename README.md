# Naive Bayes Classifier

A Naive Bayes classifier implementation for text classification using NumPy and Pandas.

## Overview

This project includes two classification tasks:
1. **Binary Classification**: SMS spam detection
2. **Multiclass Classification**: BBC news article categorization (5 categories)

## Datasets

### 1. SMS Spam Collection
- Binary classification task (Spam vs Ham)
- Located in `SMSSpamCollection` file
- Tab-separated format with labels and text

### 2. BBC News Summary
- Multiclass classification task (5 categories)
- Located in `BBCNewsSummary/NewsArticles/` directory
- Categories: Business, Entertainment, Politics, Sport, Tech
- Each category contains individual text files

## Project Structure

```
bayes_classifier/
├── Naive_bayes_clasifier.ipynb    # Main notebook with full implementation
├── SMSSpamCollection               # SMS spam dataset
├── BBCNewsSummary/
│   ├── NewsArticles/               # BBC news articles by category
│   │   ├── business/
│   │   ├── entertainment/
│   │   ├── politics/
│   │   ├── sport/
│   │   └── tech/
│   └── Summaries/
└── README.md                        # This file
```

## Installation

```bash
pip install numpy pandas nltk
python -c "import nltk; nltk.download('stopwords')"
```

## Usage

### Running the Notebook

```bash
jupyter notebook Naive_bayes_clasifier.ipynb
```

### Test Examples

**SMS Spam Detection:**
```python
testModel("See you tomorrow at lunch")  # it's a HAM
testModel("Get free money now!!")       # it's a SPAM!!
```

**BBC News Classification:**
```python
testBBCModel("news article about sports")  # it's a sport article
```
