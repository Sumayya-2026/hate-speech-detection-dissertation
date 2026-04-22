# Distinguishing Hate Speech from Offensive Language on Twitter
# Using Machine Learning Techniques

MSc Data Science Final Project - University of Hertfordshire

## Overview

This project uses machine learning to classify tweets into three categories:
- **Hate Speech**
- **Offensive Language**  
- **Neither**

**Dataset:** Davidson et al. (2017) - 24,783 labeled tweets

**Best Model:** Logistic Regression - 80.54% accuracy, 0.8008 macro F1-score

## Project Structure

```
hate-speech-detection/
├── README.md
├── requirements.txt
├── .gitignore
├── Hate_Speech_FINAL.ipynb    # Complete analysis notebook
└── labeled_data.csv            # Dataset
```

## Installation

1. Clone this repository
2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the Jupyter notebook:
```bash
jupyter notebook Hate_Speech_FINAL.ipynb
```

## Requirements

- Python 3.8+
- NumPy
- pandas
- scikit-learn
- matplotlib
- seaborn

## Methodology

1. **Data Preprocessing:** 10-stage text cleaning pipeline
2. **Class Balancing:** Random downsampling (13:1 → 1:1:1)
3. **Feature Extraction:** TF-IDF with unigrams and bigrams
4. **Models:** Logistic Regression, Linear SVM, Naive Bayes
5. **Evaluation:** 5-fold cross-validation, macro F1-score

## Results

| Model | Accuracy | Macro F1 |
|-------|----------|----------|
| Logistic Regression | 80.54% | 0.8008 |
| Linear SVM | 80.30% | 0.7975 |
| Naive Bayes | 74.59% | 0.7464 |

## Dataset

Davidson, T., Warmsley, D., Macy, M., & Weber, I. (2017). Automated Hate Speech Detection and the Problem of Offensive Language. *Proceedings of ICWSM*.

**License:** MIT

## Author

MSc Data Science Student  
University of Hertfordshire  
2026

## License

MIT License

