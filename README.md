# Sentiment Analysis on SEC 10-K Filings
**Comparing Dictionary-Based and Transformer-Based Methods**

## Overview
This study analyzes sentiment in SEC 10-K filings by comparing two approaches:
- **Lexicon-based method**: Loughran-McDonald (LM) Financial Sentiment Dictionary.
- **Transformer-based model**: FinBERT, a fine-tuned version of BERT for financial texts.

We systematically evaluated sentiment at:
- **Section level**: Item 1 (Business), Item 7 (Management Discussion), Item 7A (Quantitative Disclosures).
- **Full-document level**: Entire 10-K filings.

The project explores how well each method captures financial sentiment and discusses their strengths, weaknesses, and real-world implications.

---

## Methodology

- **Data Collection**: 10-K filings scraped from SEC EDGAR database.
- **Preprocessing**: Cleaning HTML, extracting text, tokenization, and segmentation.
- **Sentiment Analysis**:
  - **LM Method**: Computed positive, negative, and net sentiment percentages.
  - **FinBERT Model**: Classified text chunks as Positive, Neutral, or Negative, aggregated into overall scores.
- **Statistical Comparison**:
  - Pearson correlation analysis
  - Paired samples t-tests
  - Confusion matrix analysis
  - Class distribution comparison
  - Agreement rate calculation

---

## Key Results

- **Correlation**: Moderate positive correlations between LM and FinBERT (r ≈ 0.45).
- **Sentiment Scores**: FinBERT detects slightly more optimistic tones compared to LM.
- **Agreement Rates**: Ranged from 21.4% to 89.2% depending on section.
- **Confusion Matrix**: Highlighted that FinBERT is more sensitive to subtle negative cues missed by LM.

---

## Visualizations
- Correlation scatter plots between LM and FinBERT.
- Sentiment class distribution bar charts.
- Agreement rate bar chart.
- Full-document level confusion matrix.

All visualizations were generated using Matplotlib and Seaborn.

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/simransukhawani/sentiment_analysis_10K_filings.git
   cd sentiment_analysis_10K_filings
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open and run the notebook:
   ```
   code/sentiment_analysis_10k.ipynb
   ```
---

## Keywords
`Sentiment Analysis`, `Financial NLP`, `SEC 10-K Filings`, `Loughran-McDonald Lexicon`, `FinBERT`, `Transformer Models`, `Lexicon-Based Methods`, `Financial Text Mining`


## Contact

If you have any questions, feedback, or collaboration opportunities, feel free to reach out:

- 📧 Email: [simransukhawani3@gmail.com ](mailto:simransukhawani3@gmail.com)
- 🌐 GitHub: [@simransukhawani](https://github.com/simransukhawani)

---
