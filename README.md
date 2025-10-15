# Ng Rui Bin, Damien A0252828X IA3

## Overview
This project compares **Full Fine-tuning** and **LoRA (Low-Rank Adaptation)** using the **DistilBERT** model on a **financial sentiment analysis** dataset.  
The goal is to evaluate the trade-offs between performance and parameter efficiency when fine-tuning transformer models.

---

## Dataset
**Dataset:** [Twitter Financial News Sentiment](https://huggingface.co/datasets/zeroshot/twitter-financial-news-sentiment)

- 3 sentiment classes: **Bearish**, **Bullish**, **Neutral**
- Contains short financial tweets and news headlines
- Automatically downloaded via Hugging Face (no manual download needed)

---

## Setup Instructions

### 1️. Clone this repository
```bash
git clone https://github.com/daaaimes/DSA4213_IndividualAssignment3_DamienNg.git
cd DSA4213_IndividualAssignment3_DamienNg
```

### 2. Create and Activate a Virtual Environment
Uncomment according to which system OS you are using.
```bash
python -m venv env
source env/bin/activate   # macOS / Linux
# .\env\Scripts\activate  # Windows
```

### 3. Install Dependencies
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

## Running Instructions
To run the code, simply run:
```bash
python main.py
```
This will:
- Load the Twitter Financial News Sentiment dataset
- Train two models:
    - Full Fine-tuning: all model parameters updated
    - LoRA Fine-tuning: only small low-rank matrices updated
- Evaluate both models on the validation and test sets
- Print results including accuracy, F1 score, training time, and number of parameters
- Generate a comparison plot

## Files in this Directory
```bash
main.py                 # Main experiment script
main.ipynb              # Backup experiment script (if the above does not work)
requirements.txt        # Dependencies for reproducibility
README.md               # Project documentation (this file)
A0252828X_Report.pdf    # Report

```
