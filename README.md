# Maruti Stock Sentiment Analysis

A machine learning project that analyzes news headlines from MoneyControl to predict Maruti stock price movements. The system correlates financial news sentiment with historical stock data from Yahoo Finance (2020-2021).

## Overview

This project implements:
- Web scraping of financial news headlines
- Text preprocessing and sentiment analysis
- Stock price movement prediction using Random Forest classification
- Correlation analysis between news sentiment and price changes

## Features

- **News Scraping**: Automated collection of headlines from MoneyControl using BeautifulSoup
- **Data Processing**: 
  - Converts dates to standardized format
  - Combines multiple headlines per day
  - Removes special characters and converts to lowercase
- **Sentiment Analysis**:
  - Uses Bag of Words with Count Vectorization
  - Implements n-gram features (2,2)
  - Random Forest classifier for prediction
- **Stock Data**:
  - Historical data from Yahoo Finance
  - Binary classification (1 for price increase, 0 for decrease)
  - Integration with news headline dates

## Tech Stack

- Python 3.x
- pandas: Data manipulation and analysis
- scikit-learn: Machine learning implementation
- BeautifulSoup4: Web scraping
- requests: HTTP library
- matplotlib: Data visualization

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/maruti-stock-sentiment.git

## Model Performance

- Training set: 200 samples
- Test set: 35 samples
- Accuracy: 54.28%
- Detailed metrics available in confusion matrix and classification report

## Project Structure

```
├── data/
│   ├── MARUTI.NS.csv        # Stock price data
│   └── headlines.csv        # Scraped news headlines
├── src/
│   ├── scraper.py          # News scraping module
│   ├── sentiment.py        # Sentiment analysis
│   └── visualize.py        # Visualization code
├── notebooks/
│   └── analysis.ipynb      # Jupyter notebook with analysis
├── requirements.txt        # Project dependencies
└── README.md
```

## Future Improvements

- Implement more advanced NLP techniques
- Add more news sources
- Incorporate technical indicators
- Experiment with different ML models
- Real-time prediction capabilities


## Acknowledgments

- MoneyControl for financial news data
- Yahoo Finance for stock price data
- Contributors and maintainers of the libraries used

## Contact


Project Link: [https://github.com/yourusername/maruti-stock-sentiment](https://github.com/yourusername/maruti-stock-sentiment)
